# Roadmap

Each day's quiz ends with one **Part** below. Finish it, commit with a message
starting `Part N:` (for example `Part 3: add Stock subclass`), and push.
The next morning's run checks your code, gives feedback, and assigns the next part.

Status: `[ ]` not started · `[~]` in progress · `[x]` done

## Phase 1 - Core model (classes, encapsulation, static)
- [ ] Part 1: `Asset` class - ticker, name, current price; constructor, getters, validated setter for price
- [ ] Part 2: `toString`, `equals`, `hashCode` on `Asset` (two assets are equal if tickers match)
- [ ] Part 3: `Holding` class - an asset plus quantity and average cost; method for market value
- [ ] Part 4: `Account` class - cash balance, deposit/withdraw with validation, static counter for account IDs

## Phase 2 - Inheritance and abstraction
- [ ] Part 5: Make `Asset` abstract; add `Stock` and `ETF` subclasses using `super(...)`
- [ ] Part 6: `Bond` subclass with coupon rate; override an abstract `describe()` method in each subclass
- [ ] Part 7: Abstract `annualIncome()` - dividends for stocks/ETFs, coupons for bonds

## Phase 3 - Interfaces and polymorphism
- [ ] Part 8: `Priceable` and `Tradable` interfaces; implement them where they fit
- [ ] Part 9: Abstract `Order` with `MarketOrder` and `LimitOrder`; polymorphic `canExecute(price)`
- [ ] Part 10: `Portfolio` class holding a list of `Holding`s; total value computed polymorphically

## Phase 4 - Exceptions
- [ ] Part 11: Custom `InsufficientFundsException` (checked) and `InvalidOrderException` (unchecked)
- [ ] Part 12: `TradeEngine.execute(order)` - buys/sells update cash and holdings, throwing exceptions on bad trades
- [ ] Part 13: Transaction history - a `Transaction` record of every executed trade

## Phase 5 - Collections and generics
- [ ] Part 14: Generic `Repository<T>` with add / findById / getAll
- [ ] Part 15: Bounded generics - `Repository<T extends Asset>`, a generic method to find the highest-priced item
- [ ] Part 16: Market price simulator - randomly moves prices each "tick"

## Phase 6 - Finish and polish
- [ ] Part 17: Command-line menu in `Main` (buy, sell, view portfolio, advance market, history)
- [ ] Part 18: JUnit tests for `Account`, `TradeEngine`, and `Portfolio`
- [ ] Part 19: Clean up: Javadoc, README with features, how to run, and a sample session
