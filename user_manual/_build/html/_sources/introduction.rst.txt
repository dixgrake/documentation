Localizacion Dominicana
=======================

Este repositorio consolida los módulos utilizados para poder realizar facturación en República Dominicana desde los módulos de Ventas, Compra, Contable y Punto de Ventas.

En esta versión están disponibles los siguientes módulos:

- **ncf_manager**: Este módulo agrega funcionalidades para manejar numero de comprobante fiscal NCF.

        - Secuencias Preconfiguradas para manejo de todos los NCF.
        - Validación en tiempo real de comprobantes.
        - Consulta de tasas de banco en tiempo real.
        - Creación de contactos por RNC o Cédula.

- **ncf_pos**: Incorpora funcionalidades de facturación con NCF al punto de venta.
      
        - WIP: compatibilidad con impresoras fiscales
  
- **ncf_sale**: Este módulo extiende la funcionalidad del ``ncf_manager`` hacia ventas, para realizar algunas validaciones antes de crear la factura.

- **ncf_purchase**: Este módulo extiende la funcionalidad del ``ncf_manager`` hacia compras, Se agrego un nuevo campo *Diario de Compras* en proveedores si este campo está configurado, las facturas generadas para estos proveedores toman este diario de manera predeterminada.

- **dgii_report**: Este módulo extiende las funcionalidades del ``ncf_manager`` integrando los reportes de declaraciones fiscales.
          
- **ncf_invoice_template**: Este módulo sobre escribe el formato de las facturas para adaptarlo a la Norma General 06-2018 de la DGII.
            
- **external_service_addons**:

         - ``l10n_do_currency_update``: Actualiza las tasas de moneda secundaria de la compañía de los bancos dominicanos
         - ``l10n_do_rnc_validation`` : Validar RNC / Cédula del servicio externo