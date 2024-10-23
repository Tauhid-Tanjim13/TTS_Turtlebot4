# Bluetoothctl Troubleshooting Guide for Turtlebot4

If `bluetoothctl` is stuck on the message `Waiting to connect to bluetoothd...`, it indicates that the Bluetooth daemon (`bluetoothd`) is not running or there's an issue with the Bluetooth service on your system. This guide provides steps to troubleshoot and resolve the issue.


## Steps to Resolve

### 1. Check if the Bluetooth Service is Running
   Verify the status of the Bluetooth service with:
   ```
   sudo systemctl status bluetooth
```
If the service is not running (inactive or failed), start it using
```
sudo systemctl start bluetooth
```

### 2. Enable the Bluetooth Service
```sudo systemctl enable bluetooth```
