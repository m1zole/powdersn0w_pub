#ICC		= xcrun -sdk iphoneos clang
MCC		= xcrun -sdk macosx clang
MCC_FLAGS	= -I../include -Os -Wall

.PHONY: all

all:
	$(MCC) $(MCC_FLAGS) -c *.c
	ar rcs common.a *.o
	-$(RM) *.o


clean:
	-$(RM) *.a
