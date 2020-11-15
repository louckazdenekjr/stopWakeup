This should stop random wakeups from sleep/hibernation on Linux based desktop systems by disabling XHC and EHC1 based wakeup calls. Comes in the form of a systemd service. To install this:
Place the .service file into /etc/systemd/system/ and run "sudo systemctl daemon-reload && sudo systemctl start stopwakeup && sudo systemctl enable stopwakeup".
