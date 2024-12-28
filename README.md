<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>WhatsApp OTP Receiver Tool</title>
</head>
<body>
    <h1>WhatsApp OTP Receiver Tool</h1>
    <p>Developer: <strong>Jadenafrix4</strong></p>
    <h2>Installation Instructions</h2>
    <pre>
        pkg update && pkg upgrade
        pkg install git
        pkg install python
        git clone https://github.com/Jadenafrix4/whatsapp-otp-receiver.git
        cd whatsapp-otp-receiver
        python receiver.py
    </pre>
    <h2>Code for OTP Receiver</h2>
    <pre>
        #!/usr/bin/env python3

        import os
        import sys
        import time

        def main():
            try:
                # Simulate receiving OTP
                print("Listening for WhatsApp OTP...")
                while True:
                    # Here you would implement the actual logic to receive OTP
                    # For demonstration, we simulate an OTP received
                    otp = "123456"  # Simulated OTP
                    print(f"Received OTP: {otp}")
                    time.sleep(10)  # Wait for 10 seconds before checking again
            except KeyboardInterrupt:
                print("\nExiting the OTP receiver.")
                sys.exit(0)
            except Exception as e:
                print(f"An error occurred: {e}")
                sys.exit(1)

        if __name__ == "__main__":
            main()
    </pre>
    <h2>Usage</h2>
    <p>Run the following command in Termux to start the OTP receiver:</p>
    <pre>python receiver.py</pre>
    <h2>Notes</h2>
    <p>This tool is designed to work on Termux. Ensure you have the necessary permissions and configurations set up for receiving messages.</p>
</body>
</html>
