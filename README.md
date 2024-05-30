# Dell R720xd server silent fans script

Dell R720xd is a nice and cheap 2u sever, but while you are using it at home you can find it's fans are pretty loud.

Fans performance is pretty decent for high load, but in most cases while using it at home there is no need to use full fans performance which sound is pretty annoying.

# Installation
- First you need to install `ipmitool` on server to be able to read temperatures and change fan speed via this tool

- To make R720xd fans quieter just copy `dell-r720-fan-control_local.sh` somewhere to server (for example in /root) make it executable and add to cron to start once per minute.

# Setting
This script will check current server temperatures once per 10 seconds and control fan speed depending on it.

- If you find that speed is not meet your expectations you can change `correction` variable to positive or negative values to increase or reduce overall fan speed.
- Also you can change `ITERATION_SLEEP` and `ITERATION_MAX` variables to reduce / increase time between temperature checks

## Donations

You can say thanks by donating for buying pizza at:

<a href="https://www.buymeacoffee.com/astraliens" target="_blank"><img src="https://cdn.buymeacoffee.com/buttons/default-orange.png" alt="Buy Me A Pizza" height="41" width="174"></a>