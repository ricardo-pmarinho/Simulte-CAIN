PATH=~/omnetpp-5.6.2/samples/inet/

commented line 121 at PATH/src/inet/linklayer/acking/AckingMac.cc

commented line 201 at PATH/src/inet/linklayer/acking/AckingMac.cc

commented line 82 at PATH/src/inet/common/lifecycle/OperationalBase.cc
	//throw cRuntimeError("Self message '%s' received when %s is down", message->getName(), getComponentType()->getName());
added
        delete message;
to line 83 at PATH/src/inet/common/lifecycle/OperationalBase.cc

commented line 277 at PATH/src/inet/physicallayer/packetlevel/Radio.cc (throw cRuntimeError("Received frame from upper layer while already transmitting.");) and added cancelEvent(transmissionTimer);
