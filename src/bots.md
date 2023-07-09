# Bots

A `Bot` is a running instance of a `Strategy`. `Strategy` requires user input/params to create the underlying bot thread.

## Creating Bot with Wizard

1. New strategy (Button Click): SPL / USDC (dropdown option).
2. Prompt user for token ID or marketID.
3. If token ID provided, show available marketIDs for the token they gave.
4. Prompt user to choose their base wallet and quote wallet from available options.
5. Prompt user to choose their Open Orders Account, or button to create one if none exists.
6. Prompt user for additional required Strategy params.

