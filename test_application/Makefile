
GnssMetadata:
	g++ -I libsrc/API/include/ -I libsrc/API/lib/tinyxml2/ -I libsrc/API/lib/GnssMetadata/Xml/ libsrc/API/lib/tinyxml2/*.cpp libsrc/API/lib/GnssMetadata/Xml/*.cpp libsrc/API/lib/GnssMetadata/*.cpp -D LINUX -w -fmax-errors=1 -fpermissive -std=c++11 -c

GnssDecoder:
	g++ -I include/ -I libsrc/GNSSReader/include/ -I libsrc/API/include/ -I libsrc/API/lib/tinyxml2/ -I libsrc/API/lib/GnssMetadata/ -I libsrc/API/lib/GnssMetadata/Xml/ obj/*.o libsrc/GNSSReader/lib/*.cpp src/*.cpp -D LINUX -w -fmax-errors=1 -fpermissive -std=c++11 -lpthread -o test_application
