# Aes_cryptographic_tool
This Python code utilizes the `tkinter` library to create a simple graphical user interface (GUI) for text encryption using the Advanced Encryption Standard (AES) in Cipher Block Chaining (CBC) mode. Here's a summary of the code:

1. Import Libraries:
   - `tkinter`: GUI toolkit for creating the graphical interface.
   - `ttk` (Themed Tkinter): Provides access to the Tk themed widget set.
   - `cryptography.fernet.Fernet`: A symmetric encryption algorithm for securing data.

2. AES Functions:
   - `generate_aes_key()`: Generates a random AES key using Fernet.
   - `initialize_cipher_suite(key)`: Initializes the cipher suite with a given key.
   - `encrypt_text(text, cipher_suite)`: Encrypts the input text using AES-CBC.

3. GUI Creation:
   - Creates the main window using `tk.Tk()`.
   - Sets the window title, size, and makes it unresizable.
   - Creates a themed style for widget configuration.

4. Input Frame:
   - Creates an input frame to hold the input field and encryption button.
   - Configures a styled entry widget for text input with watermark.
   - Creates an "Encrypt" button to trigger encryption.

5. Perform Encryption Function:
   - Retrieves input text, generates a random AES key, and initializes the cipher suite.
   - Encrypts the input text using AES-CBC.
   - Displays the encrypted text and AES key in a read-only `Text` widget.

6. Output Text Widget:
   - Creates a `Text` widget for displaying the encrypted text and AES key.
   - Configures the widget to be read-only and sets font size and height.

7. Watermark Label:
   - Adds a label at the top-left corner of the window with information about the creator.

8. GUI Main Loop:
   - Starts the main loop using `window.mainloop()`.

The application allows the user to enter text in the input field, click the "Encrypt" button, and view the corresponding encrypted text and AES key in the output text area. The GUI is simple and user-friendly, with an adjustable input field, a button for encryption, and a display area for the results.
