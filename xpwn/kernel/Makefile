#ICC		= xcrun -sdk iphoneos clang
MCC		= xcrun -sdk macosx clang
MCC_FLAGS	= -I../include -I/opt/local/include -Os -Wall  -DHAVE_CRYPT 

.PHONY: all

all:
	$(MCC) $(MCC_FLAGS) -c *.c
	/Applications/Xcode.app/Contents/Developer/Toolchains/XcodeDefault.xctoolchain/usr/bin/ar rcs kernel.a *.o
	-$(RM) *.o


clean:
	-$(RM) *.o *.a
