# $FreeBSD$

PORTNAME=	pc-webkitviewer
PORTVERSION=	%%CHGVERSION%%
CATEGORIES=	www

MAINTAINER=	jt@ixsystems.com
COMMENT=	TrueOS QT5 Simple WebViewer

LICENSE=	BSD2CLAUSE

WRKSRC_SUBDIR=  src-qt5
MAKE_ARGS=      PREFIX=${STAGEDIR}${PREFIX}

CONFLICTS=      pcbsd-utils-[0-9]*

MAKE_JOBS_UNSAFE=yes
ONLY_FOR_ARCHS= amd64
USE_LDCONFIG=   yes
USE_QT5=        core gui network svg linguist_build \
		buildtools_build x11extras widgets multimedia
USES=           qmake shebangfix tar:xz
USE_GL+=	gl

WRKSRC_SUBDIR=  src-qt5

QMAKE_ARGS=     CONFIG+="configure"

USE_GITHUB=	yes
GH_ACCOUNT=	trueos
GH_PROJECT=	pc-webkitviewer
GH_TAGNAME=	%%GHTAG%%

.include <bsd.port.mk>
