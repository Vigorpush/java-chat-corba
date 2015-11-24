#java-corba-chat

A simple chat system using Java and CORBA.

### Setup

1. Run `orbd -ORBInitialPort 1050`
2. Move to the director containing `Conn.idl` and run `idlj -fall Conn.idl`
3. Build and run `ConnServer` in IntelliJ
4. Build and run any number of `ConnClient` in IntelliJ

If you want to build the program outside of IntelliJ, some information can be found here: [https://docs.oracle.com/javase/7/docs/technotes/guides/idl/jidlExample.html](https://docs.oracle.com/javase/7/docs/technotes/guides/idl/jidlExample.html)

### Chat Commands

The following special chat commands exist: 

* `/create foo` creates a chat room named foo
* `/join foo` joins a chat room named foo
* `/leave` leaves the current chat room
* `/list` lists all chat rooms
* `/name foo` changes the client name to foo
* `/help` lists all commands
* `/quit` quits the program

Any other text is sent as a message to the current chat room.
