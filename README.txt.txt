# Sistema POS - Ferretería Martillo 3 Golpes

Sistema de Punto de Venta (POS) y Gestión de Inventario desarrollado en Python. Diseñado específicamente para ferreterías y retail minorista, enfocado en la agilidad de venta, control estricto de stock y emisión de documentos formales.

**Desarrollador:** Cristopher Palacios  
**Versión:** 10.22 (Final Retail)  
**Año:** 2026

## 🚀 Características Principales

### 📦 Gestión de Bodega (Inventario)
- **Buscador en Tiempo Real:** Filtrado instantáneo por nombre o código de barras.
- **Gestión de Costos:** Manejo de Costo Neto, Costo + IVA y Precio de Venta.
- **Alertas Visuales:** Los productos con **Stock 0** se resaltan automáticamente en color rojo.
- **Herramienta F6:** Menú rápido para Eliminar o Modificar productos (edición completa de precios y stock).
- **Navegación:** Barra de desplazamiento lateral para inventarios extensos.

### 💰 Caja y Ventas
- **Modos de Venta:** Boleta, Factura y Cotización.
- **Cotizaciones Formales:** Generación de documentos que **no descuentan stock** ni afectan el cierre de caja.
- **Control de Carrito:**
  - Escáner de código de barras (Pistola USB).
  - Buscador manual de productos.
  - **Tecla F7:** Eliminación rápida de ítems del carrito.
- **Cálculo Automático:** Desglose de Neto e IVA (19%) en tiempo real.

### 🖨️ Impresión y Reportes
- **Impresión Térmica Directa (80mm):** Sin ventanas emergentes (Silent Print) usando motor `SumatraPDF` + `win32`.
- **Diseño Retail:** Boletas con formato de supermercado (Letra grande, Negritas, Totales gigantes).
- **Reporte de Cierre (A4):** Generación de PDF ejecutivo con KPI de ventas diarias y desglose por medio de pago.

## 🛠️ Requisitos Técnicos

El sistema requiere **Windows 10/11** y las siguientes dependencias:

### Librerías Python
```bash
pip install tk
pip install reportlab
pip install pywin32
pip install pandas openpyxl