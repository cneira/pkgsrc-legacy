# $NetBSD: Makefile,v 1.34 2017/06/05 14:22:56 ryoon Exp $

DISTNAME=	ExtUtils-F77-1.20
PKGNAME=	p5-${DISTNAME}
PKGREVISION=	2
CATEGORIES=	devel perl5
MASTER_SITES=	${MASTER_SITE_PERL_CPAN:=ExtUtils/}

MAINTAINER=	pkgsrc-users@NetBSD.org
HOMEPAGE=	http://search.cpan.org/dist/ExtUtils-F77/
COMMENT=	Perl module for determining how to link Fortran and C
LICENSE=	${PERL5_LICENSE}

USE_LANGUAGES=		fortran77
PERL5_PACKLIST=		auto/ExtUtils/F77/.packlist

.include "../../lang/perl5/module.mk"
.include "../../mk/bsd.pkg.mk"
