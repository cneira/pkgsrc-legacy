# $NetBSD: Makefile,v 1.3 2017/04/19 11:24:38 jperkin Exp $

DISTNAME=	bcollect-0.6.0
CATEGORIES=	sysutils
MASTER_SITES=	ftp://ftp.ancient-solutions.com/pub/bsdprojects/bcollect/

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://bcollect.ancient-solutions.com/
COMMENT=	Incremental remote backup tool

PKG_DESTDIR_SUPPORT=	destdir
GNU_CONFIGURE=	yes
USE_TOOLS+=	lex yacc

# Incomplete dependencies on confparser.h
MAKE_JOBS_SAFE=	no

CONF_FILES+=	${PREFIX}/share/examples/bcollect/bcollect.conf	\
		${PKG_SYSCONFDIR}/bcollect.conf

DEPENDS+=	rsync>=3.0.0:../../net/rsync

.include "../../devel/clib/buildlink3.mk"
.include "../../mk/bsd.pkg.mk"
