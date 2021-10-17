<p align="left">
  <img src="https://www.vectorlogo.zone/logos/elixir-lang/elixir-lang-icon.svg" />
</p>

# Reports Generator

Elixir algorithm exercise that processes large CSV files with Elixir Streams and generates reports based on the data.

## Measuring runtime:

**Normal version:**

```elixir
:timer.tc(fn -> ReportsGenerator.build("report_complete.csv") end)
```

**Parallel version:**

```elixir
:timer.tc(fn -> ReportsGenerator.build_from_many(["report_1.csv", "report_2.csv", "report_3.csv"]) end)
```
