# $NetBSD: Makefile,v 1.4 2017/01/03 13:23:01 jperkin Exp $

DISTNAME=	yuicompressor-2.4.8
PKGNAME=	${PYPKGPREFIX}-${DISTNAME}
CATEGORIES=	archivers python
MASTER_SITES=	${MASTER_SITE_PYPI:=y/yuicompressor/}

MAINTAINER=	rodent@NetBSD.org
HOMEPAGE=	https://bitbucket.org/sprat/yuicompressor
COMMENT=	YUI Compressor packaged for Python
LICENSE=	modified-bsd

USE_LANGUAGES=	# none

PY_PATCHPLIST=	yes
USE_JAVA=	run

post-install:
	${MV} ${DESTDIR}${PREFIX}/bin/yuicompressor \
		${DESTDIR}${PREFIX}/bin/yuicompressor${PYVERSSUFFIX} || ${TRUE}

.include "../../mk/java-vm.mk"
.include "../../lang/python/egg.mk"
.include "../../mk/bsd.pkg.mk"
