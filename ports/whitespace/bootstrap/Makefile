# Heavily borrowed from misc/instant-server and freebsddiary.
#
# $Id: Makefile,v 1.1.1.1 2008/03/24 17:13:30 asenchi Exp $
#

PORTNAME=	whitespace-bootstrap
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
		puppet:${PORTSDIR}/sysutils/puppet \
		python27:${PORTSDIR}/lang/python27 \
		rsync:${PORTSDIR}/net/rsync \
		rdate:${PORTSDIR}/sysutils/rdate \
		sudo:${PORTSDIR}/security/sudo \
		tmux:${PORTSDIR}/sysutils/tmux \
		vim:${PORTSDIR}/editors/vim \
		zsh:${PORTSDIR}/shells/zsh



# Don't let stupid programs ask for configuration.

BATCH=		YES
NO_BUILD=	YES

postinstall:

do-install:

.include <bsd.port.mk>
