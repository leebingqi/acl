include ../Makefile.in
#EXTLIBS = -lpolarssl
#EXTLIBS = -lz -liconv
#Path for SunOS
ifeq ($(findstring SunOS, $(UNIXNAME)), SunOS)
	EXTLIBS += -lz -liconv
else
	EXTLIBS += -lz
endif
ifeq ($(findstring FreeBSD, $(UNIXNAME)), FreeBSD)
	EXTLIBS += -L/usr/local/lib -liconv
endif
ifeq ($(findstring Darwin, $(UNIXNAME)), Darwin)                               
	EXTLIBS += -L/usr/lib -liconv                                          
endif
PROG = upload
