# Información legal de Deevoro

Páginas públicas de **Términos y Condiciones** y **Política de Privacidad** de
Deevoro (Plataforma de apoyo al deporte Bade S.L.).

Existen aquí porque Google —tanto la pantalla de consentimiento de OAuth como la
ficha de Google Play— exige que estos dos documentos estén en una URL pública.

## No edites estos ficheros a mano

Se **generan** desde el repositorio privado de la aplicación, con:

    npm run legales

La fuente única es `lib/textosLegales.js` en ese repositorio, que es también lo que
pinta las pantallas dentro de la app. Editar aquí crearía dos copias del mismo texto
que se separarían en silencio: exactamente el fallo que este montaje evita —las
condiciones llegaron a prometer unos gastos de gestión distintos de los que la app
cobraba, porque el texto vivía en dos sitios.

Para cambiar algo: se toca `lib/textosLegales.js`, se regenera y se copia aquí.

## El fichero CNAME no se borra

En la raíz hay un fichero `CNAME` con `legal.deevoro.com`. Es lo que ata el dominio
propio a estas páginas. Si al copiar páginas nuevas te llevas por delante ese
fichero, el dominio deja de funcionar y las URLs que Google tiene guardadas dejan
de responder, sin ningún aviso.

Al regenerar: copia solo los `.html`.
