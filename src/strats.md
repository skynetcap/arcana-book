# Strategies

The `Strategy` is an abstract class in Arcana for implementing market logic and business logic, for an onchain trading strategy, across one or more DEXs.

A number of singleton objects are available as Beans to each Strategy, notably:
- `RpcClient` - Solana RPC
- `PythManager` - Pyth Client
- `SerumManager` - OpenBook Client
- `OkHttpClient` - HTTP Client

These singleton Beans allow `Strategy` authors to access Solana functionality in their business logic.