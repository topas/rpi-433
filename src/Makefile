all: codesend RFSniffer
	
codesend: RCSwitch.o codesend.o
	$(CXX) $(CXXFLAGS) $(LDFLAGS) $+ -o ../build/$@ -lcrypt -lwiringPi -lwiringPiDev 
	
RFSniffer: RCSwitch.o RFSniffer.o
	$(CXX) $(CXXFLAGS) $(LDFLAGS) $+ -o ../build/$@ -lcrypt -lwiringPi -lwiringPiDev

clean:
	$(RM) *.o codesend RFSniffer
