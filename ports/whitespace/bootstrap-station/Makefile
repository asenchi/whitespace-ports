# Heavily borrowed from misc/instant-server and freebsddiary.
#
# $Id: Makefile,v 1.1.1.1 2008/03/24 17:13:30 asenchi Exp $
#

PORTNAME=	bootstrap-station
PORTVERSION=	0.1
PORTREVISION=	0
CATEGORIES=	misc
MASTER_SITES=	# Empty
DISTFILES=	# None

MAINTAINER=	asenchi@asenchi.com
COMMENT=	Installs a number of ports after a server installation.

RUN_DEPENDS=	bsdsar:${PORTSDIR}/sysutils/bsdsar \
		bash:${PORTSDIR}/shells/bash \
		ezjail:${PORTSDIR}/sysutils/ezjail \
		git:${PORTSDIR}/devel/git \
		openntpd:${PORTSDIR}/net/openntpd \
		perl5.10:${PORTSDIR}/lang/perl5.10 \
		python27:${PORTSDIR}/lang/python27 \
		rdate:${PORTSDIR}/sysutils/rdate \
		redis:${PORTSDIR}/databases/redis \
		rsync:${PORTSDIR}/net/rsync \
		sudo:${PORTSDIR}/security/sudo \
		tmux:${PORTSDIR}/sysutils/tmux \
		vim:${PORTSDIR}/editors/vim \
		zsh:${PORTSDIR}/shells/zsh



# Don't let stupid programs ask for configuration.
BATCH=		YES
NO_BUILD=	YES

post-install:
	echo 'security.jail.allow_raw_sockets=1' >> /etc/sysctl.conf

do-install:

.include <bsd.port.mk>
