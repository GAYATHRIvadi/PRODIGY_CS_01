# PRODIGY_CS_01
def caesar_encrypt(plaintext, shift):
    encrypted_text = ""
    for char in plaintext:
        if char.isalpha()
            start = ord('A') if char.isupper() else ord('a')
            shifted_char = chr(start + (ord(char) - start + shift) % 26)
            encrypted_text += shifted_char
        else:
            encrypted_text += char
    return encrypted_text
def caesar_decrypt(ciphertext, shift):
     return caesar_encrypt(ciphertext, -shift)
def main():
    while True:
        choice = input("Would you like to encrypt or decrypt a message? (Enter 'encrypt' or 'decrypt', or 'exit' to quit): ").strip().lower() 
        if choice == 'exit':
            print("Exiting the program.")
            break
        elif choice not in ['encrypt', 'decrypt']:
            print("Invalid choice. Please enter 'encrypt', 'decrypt', or 'exit'.")
            continue
        message = input("Enter the message: ")
        shift = int(input("Enter the shift value (integer): "))
        if choice == 'encrypt':
            result = caesar_encrypt(message, shift)
            print(f"Encrypted message: {result}")
        elif choice == 'decrypt':
            result = caesar_decrypt(message, shift)
            print(f"Decrypted message: {result}")

if __name__ == "__main__":
    main()

