# ghci-runner

Use this module to build your own version of the Yesod scaffolding's
DevelMain.hs. Do this by creating a module that wraps a call to update
with proper arguments, e.g. a test-main for the library. Generally
you'll re-export shutdown as-is.

Then you can quickly iterate and rerun the computation. Start @stack
ghci@, :load your module, and run the computation that is the wrapped
version of update. After hacking some, :reload and rerun the
computation.

For an example, see Snowdrift's dev/Runner.hs (FIXME: Add a link once
it's merged).
