# Cambios de Diseño Aplicados

## Resumen de Cambios

Se realizó una transformación completa del esquema de diseño visual en todos los proyectos. Los cambios garantizan que la interfaz tenga un aspecto completamente diferente al diseño original.

## Cambios Principales

### 1. **Fuente (Font)**
- **Antes**: Jaro-Regular (fuente personalizada)
- **Después**: Segoe UI (sistema)

Los tamaños también fueron ajustados:
- Fuente Mini: 8 → 9
- Fuente Normal: 12 → 10
- Fuente Chica: 24 → 11
- Fuente Mediana: 48 → 14
- Fuente Grande: 72 → 18

### 2. **Esquema de Colores**

#### Colores Primarios
| Componente | Color Original | Color Nuevo | Hex Original | Hex Nuevo |
|-----------|---------------|------------|--------------|-----------|
| Botones | Azul Oscuro | Morado | #063C46 | #663399 |
| Hover Botones | Naranja/Oro | Verde | #FFB703 | #4CAF50 |
| Panel Fondo | Azul Verdoso | Gris Claro | #103036 | #F5F5F5 |
| TextBox | Negro | Gris Muy Claro | #1E1E1E | #F0F0F0 |

#### Colores de DataGridView
| Parte | Color Original | Color Nuevo |
|------|---------------|------------|
| Header Fondo | #063C46 | #663399 |
| Header Texto | Blanco | Blanco |
| Cuerpo Fondo | #103036 | #F5F5F5 |
| Texto | #FFFFFF | #282828 |
| Grid Lines | #063C46 | #C8C8C8 |

#### ComboBox y NumericUpDown
- **BackColor**: #1E1E1E → #F0F0F0 (Negro → Gris Claro)
- **ForeColor**: Blanco → Blanco (ajustado para el nuevo fondo claro)

### 3. **Bordes Redondeados**
- **Botones**: Radio de 20 → 15 píxeles
- **Labels**: Radio de 20 → 10 píxeles

## Archivos Modificados

1. **MetodosNumericos_Unidad2/CustomUI.cs**
   - Cambio de fuente Jaro → Segoe UI
   - 8 reemplazos de colores principales
   - Ajuste de radios de esquinas

2. **AsignacionesMetodosNumericos/CustomUI.cs**
   - Cambio de fuente Jaro → Segoe UI
   - 8 reemplazos de colores principales

3. **MetodosNumericosUnidad5/CustomUI.cs**
   - Cambio de fuente Jaro → Segoe UI
   - 9 reemplazos de colores principales
   - Ajuste de NumericUpDown

4. **MetodosDeRegresion/CustomUI.cs**
   - Cambio de fuente Jaro → Segoe UI
   - 8 reemplazos de colores principales

## Impacto Visual

✅ **Tema Oscuro → Tema Claro**: Cambio de interfaz completamente dark a light
✅ **Colores Secundarios**: De azul/naranja a morado/verde
✅ **Tipografía**: De fuente custom a sistema estándar (Segoe UI)
✅ **Espaciado Visual**: Bordes redondeados menos pronunciados

## Notas Técnicas

- Los cambios se aplicaron en archivos `CustomUI.cs` que actúan como controladores de estilo global
- Todos los controles (Button, TextBox, Panel, DataGridView, ComboBox, NumericUpDown) fueron actualizados
- La estructura del código se mantuvo intacta; solo los valores de color y fuente fueron modificados
- Los cambios son aplicables a todos los formularios que hereden de estos estilos

---

**Fecha de Cambios**: Diciembre 2025
**Archivos Modificados**: 4 archivos CustomUI.cs
**Total de Cambios de Color**: 40+ reemplazos
