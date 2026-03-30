# Pagina-web-risss
Pagina web Mzzr
# Mazzoris

Proyecto Django para el portal de Mazzoris y el procesamiento de estados de cuenta bancarios en PDF.

## Estado actual
- Landing p�blica con acceso a login.
- Dashboard privado para cargar PDFs.
- Parser BBVA ajustado con validaci�n de cuadre contra saldo inicial, dep�sitos, retiros y saldo final del PDF.
- Exportaci�n a Excel con hojas `Movimientos` y `Resumen`.

## Requisitos
- Python 3.11 o superior.
- Dependencias de `requirements.txt`.

## Instalaci�n local recomendada
1. Crear un entorno virtual nuevo.
2. Instalar dependencias.
3. Copiar `.env.example` a `.env` y ajustar valores.
4. Ejecutar migraciones.
5. Crear un superusuario con `python manage.py createsuperuser`.
6. Iniciar el servidor con `python manage.py runserver`.

## Dependencias principales
- Django
- pandas
- pdfplumber
- openpyxl
- Pillow

## Notas
- El script `create_superuser.py` contiene credenciales de desarrollo y no debe usarse en producci�n.
- El parser de otros bancos se mantuvo intacto para no interferir con los reemplazos que planeas hacer despu�s.
