ADD_LIBRARY(ipv6_dhcp SHARED dhcpv6.c dhcpv6_packet.c)
ADD_LIBRARY(ipv6_nd SHARED nd.c)

INSTALL(TARGETS ipv6_dhcp ipv6_nd
	LIBRARY DESTINATION lib${LIB_SUFFIX}/accel-ppp
)

