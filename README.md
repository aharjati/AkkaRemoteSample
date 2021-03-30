# AkkaRemoteSample
akka remote example with scala


Running the Code
----------------

Follow these steps to run the code:

1. `cd` into the _HelloRemote_ directory.
1. Type `sbt run` to start the remote actor system.
1. In a separate terminal window, `cd` into the _HelloLocal_ directory.
1. Type `sbt run` to start the local actor system.

When the local actor system starts, it will send an initial message
to the remote actor system. The remote actor will send a reply through
its `sender` reference, and this will continue five times. When the
action stops, stop each system by pressing Ctrl-C.

