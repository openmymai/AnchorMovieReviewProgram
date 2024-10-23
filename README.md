## Anchor Movie Review Program

Anchor makes invoking other Solana programs easier, 
especially if the program you're invoking is also an Anchor program whose crate you can access.

## Cross Program Invocations (CPIs) with Anchor
CPIs allow programs to invoke instructions on other programs using the ```invoke``` or ```invoke_signed``` functions. 
This allows new programs to build on top of existing programs (we call that composability).

While making CPIs directly using ```invoke``` or ```invoke_signed``` is still an option, Anchor also provides a simplified way to make CPIs by using a ```CpiContext```

- Anchor provides a simplified way to create CPIs using a CpiContext
- Anchor's cpi feature generates CPI helper functions for invoking instructions on existing Anchor programs
- If you do not have access to CPI helper functions, you can still use invoke and invoke_signed directly
- The error_code attribute macro is used to create custom Anchor Errors
