# OnOff
Sends a message 4 days then 3 days off.

## Installation

1. Download [`OnOff.zip`](https://raw.githubusercontent.com/ingig/OnOff/main/OnOff.zip) from this repository or clone the repository.
2. Ensure you have Plang installed on your system. If not, install it from [PLangHQ releases](https://github.com/PLangHQ/plang/releases).
3. Extract the downloaded zip file and navigate to the extracted directory.

## Usage

You need to have a messaging client on your phone to recieve a message. Use [Amethyst (Android)](https://play.google.com/store/apps/details?id=com.vitorpamplona.amethyst&hl=en&gl=US) or [Damus (iPhone)](https://apps.apple.com/us/app/damus/id1628663131). You need to find you public address, it starts with `npub`

## Start the application
Navigate to the OnOff folder in your terminal/command, and run this command
```bash
plang
```

You will be asked to 

You can modify the message and the time it is sent by changing the code of the application.

To change the time, change the line `- every day at 9 am, call CheckToSend` in `Start.goal`. Here are some examples
- `- only on working days at 15:23, call CheckToSend`
- `- every monday at 10, call CheckToSend`
- `- every other day at 9pm, call CheckToSend`

To change the message, simply change the text `"This is a reminder"` to what ever you want.

If you change the code, you MUST build the code so it will run with your new instructions.

Navigate to the OnOff folder in the terminal/command, and type in 
```bash
plang build
```
> [!CAUTION]
> **Heads up: Building costs money**
> When build the plang code it is going to cost a little bit of money, this is usually around $0.01 - $0.03. You will be asked to purchase credits the first time you use it.