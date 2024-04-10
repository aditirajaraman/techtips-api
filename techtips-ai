# This is a sample Python script.
from openai import OpenAI
import os

# Press Shift+F10 to execute it or replace it with your code.
# Press Double Shift to search everywhere for classes, files, tool windows, actions, and settings.


def print_hi(name):
    # Use a breakpoint in the code line below to debug your script.
    print(f'Hi, {name}')  # Press Ctrl+F8 to toggle the breakpoint.


# Press the green button in the gutter to run the script.
if __name__ == '__main__':
    print_hi('PyCharm')
    secret_key  = os.environ['OPENAPI_KEY']
    client = OpenAI(api_key=secret_key)
    # completion = client.chat.completions.create(
    #     model="gpt-3.5-turbo",
    #     messages=[
    #         {"role": "system",
    #          "content": "You are a poetic assistant, skilled in explaining complex programming concepts with creative flair."},
    #         {"role": "user", "content": "Compose a poem that explains the concept of recursion in programming."}
    #     ]
    # )

    client = OpenAI(api_key=secret_key)
    completion = client.chat.completions.create(
        model="gpt-3.5-turbo",
        messages=[
            {"role": "system",
             "content": "Can you identify any bugs in this [python] code snippet: [num1 = 1.5 num2 = 'Hello' sum = num1 + num2 print('The sum of {0} and {1} is {2}'.format(num1, num2, sum))]?."}
        ]
    )
    print(completion.choices[0].message)

    # This program adds two numbers

    # num1 = 1.5
    # num2 = "Hello"
    # sum = num1 + num2
    # print('The sum of {0} and {1} is {2}'.format(num1, num2, sum))
