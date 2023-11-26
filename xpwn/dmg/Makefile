#ICC		= xcrun -sdk iphoneos clang
MCC		= xcrun -sdk macosx clang
MCC_FLAGS	= -I../include -I/opt/local/include -Os -Wall  -DHAVE_CRYPT 

.PHONY: all

all:
	$(MCC) $(MCC_FLAGS) -c *.c
	ar rcs dmg.a *.o
	-$(RM) *.o


clean:
	-$(RM) *.o *.a
