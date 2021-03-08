# stopwakeup 

This should stop random wakeups from sleep/hibernation on Linux based desktop systems by disabling EHC1 and XHC based wakeup calls. The identifiers may need to be modified according to cat /proc/acpi/wakeup depending on the hardware in use. Comes in the form of a systemd service. To install this:
Place the .service file into /etc/systemd/system/ and run "sudo systemctl daemon-reload && sudo systemctl start stopwakeup && sudo systemctl enable stopwakeup".
