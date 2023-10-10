# Login Authentication using Streamlit and YAML Configuration

This Python script demonstrates how to implement a simple login authentication system using the Streamlit framework and YAML configuration. It allows users to log in and log out with authentication checks.

## Prerequisites

Before running the script, ensure that you have the following prerequisites installed:

- Python
- Streamlit
- PyYAML

You can install Streamlit and PyYAML using pip:

```bash
pip install streamlit pyyaml
```

## Getting Started

1. Clone the repository to your local machine.

2. Create a `config.yaml` file in the same directory as the script to store configuration details. The `config.yaml` file should have the following structure:

```yaml
credentials:
  username: your_username
  password: your_password
cookie:
  name: your_cookie_name
  key: your_cookie_key
  expiry_days: 30  # Change this to your desired expiration time in days
preauthorized: true  # Set to 'true' if you want to enable pre-authorized access
```

3. Run the Streamlit app using the following command:

```bash
streamlit run your_script_name.py
```

4. Access the Streamlit app in your web browser.

## Usage

- When you access the Streamlit app, you will be presented with a login form.

- Enter your username and password as specified in the `config.yaml` file.

- If the login is successful, you will see a welcome message with your username.

- You can log out by clicking the "Logout" button.

## Configuration

- Update the `config.yaml` file to configure the login credentials, cookie settings, and pre-authorization options.

- Adjust the `expiry_days` value in the `config.yaml` file to control the expiration time for the login cookie.

## Note

This is a simple demonstration of login authentication using Streamlit and YAML configuration. Depending on your use case, you may want to enhance security and error handling.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

Replace `your_username`, `your_password`, `your_cookie_name`, `your_cookie_key`, and other placeholders with your actual values.

Make sure to include the necessary explanations and customize the README according to your project's specific needs.
