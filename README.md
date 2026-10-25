# Coffee Machine Simulator

An object-oriented command-line simulation of a coffee machine. Users can order drinks, insert virtual coins, inspect resources, and shut down the machine.

## Features

- Latte, espresso, and cappuccino menu
- Ingredient availability checks
- Coin processing and change calculation
- Resource and profit reports
- Object-oriented separation of menu, coffee-making, and payment responsibilities

## Run

```bash
python main.py
```

Commands available at the prompt include the drink names, `report`, and `off`. No third-party packages are required.

## Structure

- `main.py` — application loop
- `menu.py` — drink definitions and lookup
- `coffee_maker.py` — resource tracking and drink preparation
- `money_machine.py` — coin and payment handling
