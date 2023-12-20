# Curl-like HTTP Client

This is a simple curl-like HTTP client implemented in Python. It allows you to send HTTP requests to a specified URL and receive the response.

I created this program was designed based on a challenge on the "Coding Challenges" website: https://codingchallenges.fyi/challenges/challenge-curl

## Usage

To use this program, follow the steps below:

1. Make sure you have Python installed on your machine.

2. Clone or download the repository to your local machine.

3. Open a terminal or command prompt and navigate to the project directory.

4. Execute the program by running the following command:
     ```
     python main.py [options] url
     ```

     Replace `[options]` with any of the following:

     - `-v` or `--verbose`: Enable verbose output.
     - `-X METHOD` or `--method METHOD`: Specify the HTTP method (default is GET).
     - `-d DATA` or `--data DATA`: Specify the data to send in the request body.
     - `-H HEADER` or `--header HEADER`: Specify additional headers.

     Replace `url` with the URL to send the request to.

5. The program will send the HTTP request and display the response.

## Examples

Here are some examples of how to use the program:

- Send a GET request to a URL:
    ```
    python main.py -v -X GET https://example.com/get
    ```

- Send a POST request with data and headers:
    ```
    python main.py -v -X POST https://example.com/post -d '{"key": "value"}' -H "Content-Type: application/json"
    ```

- Enable verbose output:
    ```
    python main.py -v https://example.com/get
    ```

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
