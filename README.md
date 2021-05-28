disabled_contracts: a stub implementation of https://crates.io/crates/contracts
===============================================================================

The contract macros are useful for development.  However, it's
important for performance sensitive code to obviously not incur
any overhead from the annotations.

The stub macros in this crate help achieve that: code can switch
between that and the real contracts crate depending on features, and
the contract code does not even have to build anymore, so any
helpers for the checking logic can also be conditionalised.
