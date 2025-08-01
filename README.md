## 🌐 Language / 语言 / Språk

- [English](#english) /  [中文](#中文) /  [Svenska](#svenska)

---

# English <a name="english"></a>
## Automatic Catalog Generator (V1.1)

This is a powerful, offline-first, browser-based tool designed to automatically generate professional, print-ready A4 product catalogs. It dynamically creates pages by merging data from an Excel spreadsheet with corresponding product images, offering extensive customization options to fit your brand identity.

The entire process runs locally in your web browser, meaning no software installation is required, and your data remains private on your computer.

### Core Features

  * **Data-Driven Generation**: Populates catalog content directly from an `.xlsx` file.
  * **Intelligent Image Matching**:
      * Automatically links and displays product images by matching the image filename with the `SKU` from the Excel file.
      * Automatically displays country flags by matching the flag's filename with the `origin` text from the Excel file.
  * **Dual Design Modes**:
      * **Promotion Mode**: A sales-focused layout featuring a prominent, customizable price tag, brand name, and country of origin flags.
      * **New Arrivals Mode**: A clean, modern layout that hides the price, highlighting the product, brand, and origin in a stylish manner.
  * **Dynamic & Responsive Layout**: The tool intelligently adjusts the size and arrangement of product cards to beautifully display anywhere from 1 to 9 products per page.
  * **Advanced Customization**:
      * **Text**: Edit promotional titles, dates, and footer content using a rich text editor with options for font, size, color, and style (bold, italic, underline).
      * **Branding**: Upload custom images for the header logo, footer image, full-page background, header background, and even the price tag background.
  * **Performance Optimized**: On-the-fly image compression helps reduce file sizes and ensures the tool runs smoothly, even with many high-resolution images.
  * **User-Friendly Interface**: Features a live preview that updates instantly, zoom controls for detailed inspection, and a status panel that provides feedback and error messages (e.g., missing images).
  * **Print & PDF Export**: Generates a clean A4 layout ready for printing or saving as a high-quality PDF directly from the browser's print dialog.

### Excel Data Format

To use the tool, your `.xlsx` file should contain a sheet with the following columns. The column headers are case-insensitive.

| Column Header | Required | Description                                                                                                                              | Example          |
| :------------ | :------- | :--------------------------------------------------------------------------------------------------------------------------------------- | :--------------- |
| `page`        | **Yes** | The page number where this product will appear. Products with the same page number will be on the same page.                                | `1`              |
| `sku`         | **Yes** | **Stock Keeping Unit**. This is the unique ID for the product. It **must** exactly match the product image's filename.                  | `2327`           |
| `name`        | Yes      | The name of the product.                                                                                                                 | `Coconut Milk`   |
| `size`        | Yes      | The size, weight, or packaging information for the product.                                                                              | `6x2900ml`       |
| `brand`       | No       | The brand name of the product. Displayed in both modes.                                                                                  | `Aroy-D`         |
| `origin`      | No       | The country of origin. To display multiple flags, separate country names with a comma. The names must match the flag image filenames.      | `Thailand,Vietnam` |
| `price`       | No       | The product price. This is only displayed in "Promotion" mode.                                                                           | `83.90`          |
| `bbd`         | No       | Best Before Date. Displayed as a small overlay on the product image if provided.                                                         | `2026-12-31`     |
| `unit`        | No       | The unit for the price (e.g., "st", "kg", "pack"). Displayed on the price tag in "Promotion" mode.                                         | `st`             |
| `remark`      | No       | A short promotional remark (e.g., "Hot Sale", "New\!"). Displayed as a small overlay on the product image if provided.                      | `Hot Sale`       |

*You can download a pre-filled template by clicking the "Download Template" button in the application.*

### Detailed User Guide

**Step 1: Upload Excel File**

1.  Prepare your product data in an `.xlsx` file according to the format described above.
2.  On the control panel, click **Choose File** under "Step 1: Upload Product Information" and select your file.
3.  The filename will appear next to the button, and the status panel will confirm if the data was parsed successfully.

**Step 2: Upload Image Files**

1.  **Product Images**: Ensure your product image filenames exactly match the `sku` in your Excel file (e.g., `2327.jpg`).
2.  **Origin Flags (Optional)**: If you use the `origin` column, ensure your flag image filenames match the country names (e.g., `Thailand.png`, `Vietnam.png`).
3.  Click **Choose Files** under "Step 2: Upload Product Pictures" and select all your product images.
4.  To upload flags, click **Choose Files** next to "Origin Flags" in the "Customize Appearance" section and select your flag images.

**Step 3: Configure Catalog Mode and Titles**

1.  Enter a date or general title in the **Promotion Date** field (e.g., "July 2025 Special").
2.  Click on the **Promotion** or **New Arrivals** tab to select the catalog's design mode.
3.  Fill in the corresponding title for the selected mode (e.g., "Kampanj" for Promotion, "NYHETER" for New Arrivals).

**Step 4: Customize Footer**

1.  Click inside the text box under **Custom Footer Text**.
2.  Use the toolbar to make text **Bold**, *Italic*, or \<u\>Underlined\</u\>.
3.  Change the font family, font size, and text color using the dropdown menus and color picker. Your changes will appear in the live preview.

**Step 5: Customize Appearance**
This section lets you fully brand your catalog. For best results, use the recommended image sizes.

  * **Header Logo**: Your company logo. (Recommended: 400x100 pixels)
  * **Header BG**: A background for the title area. (Recommended: 600x100 pixels)
  * **Page BG**: A background for the entire A4 page. (Recommended: 1240x1754 pixels)
  * **Price Tag BG**: A custom background for the price tag in Promotion mode. (Recommended: 100x100 pixels)
  * **Origin Flags**: Your collection of country flag images.
  * **Footer Image**: A logo or image to appear in the footer. (Recommended: 100x100 pixels)

**Step 6: Preview and Export**

1.  Use the **Zoom Preview** slider and buttons (`+` / `-`) to inspect the catalog pages closely.
2.  Check the **status panel** at the bottom of the controls for any error messages, such as missing images.
3.  When you are satisfied, click the **Print or Save as PDF** button.
4.  In the browser's print dialog, choose your printer or select **"Save as PDF"** as the destination to get a digital file.

-----

# 中文 (Chinese) <a name="中文"></a>

## 自动目录生成器 (V1.1)

这是一个功能强大、离线优先、基于浏览器的工具，旨在自动生成专业的、可供打印的A4产品目录。它通过合并Excel电子表格中的数据与相应的产品图片来动态创建页面，并提供广泛的自定义选项以适应您的品牌形象。

整个过程都在您的本地浏览器中运行，这意味着无需安装任何软件，您的数据将安全地保留在您自己的计算机上。

### 核心功能

  * **数据驱动生成**: 直接从 `.xlsx` 文件中读取内容来填充目录。
  * **智能图片匹配**:
      * 通过将图片文件名与Excel文件中的 `SKU` (商品编码) 进行匹配，自动链接并显示产品图片。
      * 通过将旗帜图片的文件名与Excel文件中的 `origin` (原产地) 文本进行匹配，自动显示国旗。
  * **双设计模式**:
      * **促销模式**: 一种以销售为重点的布局，具有突出的、可自定义的价格标签、品牌名称和原产国国旗。
      * **新品模式**: 一种干净、现代的布局，隐藏了价格，以时尚的方式突出产品、品牌和产地。
  * **动态响应式布局**: 工具能智能地调整产品卡片的大小和排列，以完美地在每页上展示1到9个产品。
  * **高级自定义选项**:
      * **文本**: 使用富文本编辑器编辑促销标题、日期和页脚内容，提供字体、大小、颜色和样式（粗体、斜体、下划线）选项。
      * **品牌化**: 可为页眉Logo、页脚图片、整页背景、页眉背景、甚至价格标签背景上传自定义图片。
  * **性能优化**: 即时图像压缩有助于减小文件大小，并确保即使有许多高分辨率图像，工具也能流畅运行。
  * **用户友好的界面**: 具有即时更新的实时预览、用于详细检查的缩放控件，以及提供反馈和错误消息（如缺少图片）的状态面板。
  * **打印与PDF导出**: 直接从浏览器的打印对话框中，生成可供打印或另存为高质量PDF的A4页面。

### Excel 数据格式

要使用此工具，您的 `.xlsx` 文件应包含一个具有以下列的工作表。列标题不区分大小写。

| 列标题 | 是否必需 | 描述                                                                                                                               | 示例             |
| :------- | :------- | :--------------------------------------------------------------------------------------------------------------------------------- | :--------------- |
| `page`   | **是** | 该产品将出现的页码。具有相同页码的产品将显示在同一页上。                                                                         | `1`              |
| `sku`    | **是** | **库存单位 (Stock Keeping Unit)**。这是产品的唯一ID。它 **必须** 与产品图片的文件名完全匹配。                                      | `2327`           |
| `name`   | 是       | 产品名称。                                                                                                                         | `Coconut Milk`   |
| `size`   | 是       | 产品的尺寸、重量或包装信息。                                                                                                       | `6x2900ml`       |
| `brand`  | 否       | 产品品牌名称。在两种模式下都会显示。                                                                                               | `Aroy-D`         |
| `origin` | 否       | 原产国。要显示多个国旗，请用逗号分隔国家名称。国家名称必须与国旗图片的文件名匹配。                                                 | `Thailand,Vietnam` |
| `price`  | 否       | 产品价格。仅在“促销模式”下显示。                                                                                                   | `83.90`          |
| `bbd`    | 否       | **最佳赏味期 (Best Before Date)**。如果提供，将作为小图层显示在产品图片上。                                                        | `2026-12-31`     |
| `unit`   | 否       | 价格的单位（例如“st”, “kg”, “pack”）。在“促销模式”下显示在价格标签上。                                                             | `st`             |
| `remark` | 否       | 简短的促销语（例如“热卖”, “新品\!”）。如果提供，将作为小图层显示在产品图片上。                                                      | `Hot Sale`       |

*您可以通过点击应用程序中的“下载模板 (Download Template)”按钮来下载一个预先填充好的模板。*

### 详细用户指南

**第一步：上传Excel文件**

1.  根据上述格式，在 `.xlsx` 文件中准备您的产品数据。
2.  在控制面板的“第一步：上传产品信息”下，点击 **选择文件 (Choose File)** 并选择您的文件。
3.  文件名将出现在按钮旁边，状态面板将确认数据是否成功解析。

**第二步：上传图片文件**

1.  **产品图片**：确保您的产品图片文件名与Excel中的 `sku` 完全匹配（例如 `2327.jpg`）。
2.  **原产国国旗 (可选)**：如果您使用了 `origin` 列，请确保您的国旗图片文件名与国家名称匹配（例如 `Thailand.png`, `Vietnam.png`）。
3.  在“第二步：上传产品图片”下点击 **选择文件 (Choose Files)** 并选择您所有的产品图片。
4.  要上传国旗，请在“自定义外观”部分中，点击“原产国国旗 (Origin Flags)”旁边的 **选择文件 (Choose Files)** 并选择您的国旗图片。

**第三步：配置目录模式和标题**

1.  在 **促销日期 (Promotion Date)** 字段中输入日期或通用标题（例如“2025年七月特惠”）。
2.  点击 **促销 (Promotion)** 或 **新品 (New Arrivals)** 标签页，以选择目录的设计模式。
3.  为所选模式填写相应的标题（例如，促销模式填“Kampanj”，新品模式填“NYHETER”）。

**第四步：自定义页脚**

1.  在 **自定义页脚文本 (Custom Footer Text)** 下的文本框内点击。
2.  使用工具栏使文本变为 **粗体**、*斜体* 或\<u\>下划线\</u\>。
3.  使用下拉菜单和颜色选择器更改字体、字号和文本颜色。您的更改将显示在实时预览中。

**第五步：自定义外观**
此部分可让您完全品牌化您的目录。为获得最佳效果，请使用推荐的图片尺寸。

  * **页眉Logo (Header Logo)**：您的公司Logo。(推荐：400x100 像素)
  * **页眉背景 (Header BG)**：标题区域的背景。(推荐：600x100 像素)
  * **页面背景 (Page BG)**：整个A4页面的背景。(推荐：1240x1754 像素)
  * **价格标签背景 (Price Tag BG)**：促销模式下价格标签的自定义背景。(推荐：100x100 像素)
  * **原产国国旗 (Origin Flags)**：您的国旗图片集合。
  * **页脚图片 (Footer Image)**：出现在页脚的Logo或图片。(推荐：100x100 像素)

**第六步：预览和导出**

1.  使用 **缩放预览 (Zoom Preview)** 滑块和按钮 (`+` / `-`) 来仔细检查目录页面。
2.  检查控件底部的 **状态面板**，看是否有任何错误消息，例如缺少图片。
3.  当您满意后，点击 **打印或另存为PDF (Print or Save as PDF)** 按钮。
4.  在浏览器的打印对话框中，选择您的打印机或选择 **“另存为PDF”** 作为目标，以获取数字文件。

-----

# Svenska (Swedish) <a name="svenska"></a>

## Automatisk Produktkatalog Generator (V1.1)

Detta är ett kraftfullt, offline-först, webbläsarbaserat verktyg som är utformat för att automatiskt generera professionella, utskriftsklara A4-produktkataloger. Det skapar dynamiskt sidor genom att slå samman data från ett Excel-kalkylblad med motsvarande produktbilder och erbjuder omfattande anpassningsalternativ för att passa din varumärkesidentitet.

Hela processen körs lokalt i din webbläsare, vilket innebär att ingen programinstallation krävs och din data förblir privat på din dator.

### Kärnfunktioner

  * **Datadriven Generering**: Fyller katalogens innehåll direkt från en `.xlsx`-fil.
  * **Intelligent Bildmatchning**:
      * Länkar och visar automatiskt produktbilder genom att matcha bildens filnamn med `SKU` från Excel-filen.
      * Visar automatiskt nationsflaggor genom att matcha flaggans filnamn med `origin`-texten från Excel-filen.
  * **Dubbla Designlägen**:
      * **Kampanjläge**: En säljfokuserad layout med en framträdande, anpassningsbar prislapp, varumärke och ursprungsflaggor.
      * **Nyhetsläge**: En ren, modern layout som döljer priset och framhäver produkten, varumärket och ursprunget på ett stilfullt sätt.
  * **Dynamisk & Responsiv Layout**: Verktyget justerar intelligent storleken och arrangemanget av produktkort för att vackert visa allt från 1 till 9 produkter per sida.
  * **Avancerad Anpassning**:
      * **Text**: Redigera kampanjtitlar, datum och sidfotens innehåll med en textredigerare som har alternativ för typsnitt, storlek, färg och stil (fet, kursiv, understruken).
      * **Varumärkesprofilering**: Ladda upp anpassade bilder för sidhuvudets logotyp, sidfotens bild, helsidesbakgrund, sidhuvudets bakgrund och till och med prislappens bakgrund.
  * **Prestandaoptimerad**: Bildkomprimering i realtid hjälper till att minska filstorlekar och säkerställer att verktyget körs smidigt, även med många högupplösta bilder.
  * **Användarvänligt Gränssnitt**: Har en live-förhandsgranskning som uppdateras omedelbart, zoomkontroller för detaljerad inspektion och en statuspanel som ger feedback och felmeddelanden (t.ex. saknade bilder).
  * **Utskrift & PDF-export**: Genererar en ren A4-layout redo för utskrift eller för att sparas som en högkvalitativ PDF direkt från webbläsarens utskriftsdialog.

### Excel-dataformat

För att använda verktyget bör din `.xlsx`-fil innehålla ett ark med följande kolumner. Kolumnrubrikerna är inte skiftlägeskänsliga.

| Kolumnrubrik | Krävs   | Beskrivning                                                                                                                              | Exempel          |
| :----------- | :------ | :--------------------------------------------------------------------------------------------------------------------------------------- | :--------------- |
| `page`       | **Ja** | Sidnumret där denna produkt ska visas. Produkter med samma sidnummer hamnar på samma sida.                                               | `1`              |
| `sku`        | **Ja** | **Stock Keeping Unit** (artikelnummer). Detta är produktens unika ID. Det **måste** exakt matcha produktbildens filnamn.                   | `2327`           |
| `name`       | Ja      | Produktens namn.                                                                                                                         | `Coconut Milk`   |
| `size`       | Ja      | Produktens storlek, vikt eller förpackningsinformation.                                                                                  | `6x2900ml`       |
| `brand`      | Nej     | Produktens varumärke. Visas i båda lägena.                                                                                               | `Aroy-D`         |
| `origin`     | Nej     | Ursprungsland. För att visa flera flaggor, separera ländernas namn med ett kommatecken. Namnen måste matcha flaggbildernas filnamn.         | `Thailand,Vietnam` |
| `price`      | Nej     | Produktens pris. Visas endast i "Kampanjläge".                                                                                           | `83.90`          |
| `bbd`        | Nej     | **Bäst-före-datum**. Visas som en liten text på produktbilden om det anges.                                                              | `2026-12-31`     |
| `unit`       | Nej     | Enheten för priset (t.ex. "st", "kg", "pack"). Visas på prislappen i "Kampanjläge".                                                       | `st`             |
| `remark`     | Nej     | En kort kampanjkommentar (t.ex. "Rea", "Nyhet\!"). Visas som en liten text på produktbilden om det anges.                                   | `Hot Sale`       |

*Du kan ladda ner en förifylld mall genom att klicka på knappen "Download Template" i applikationen.*

### Detaljerad Användarhandbok

**Steg 1: Ladda upp Excel-fil**

1.  Förbered din produktdata i en `.xlsx`-fil enligt formatet som beskrivs ovan.
2.  På kontrollpanelen, klicka på **Välj fil (Choose File)** under "Steg 1: Ladda upp produktinformation" och välj din fil.
3.  Filnamnet visas bredvid knappen, och statuspanelen kommer att bekräfta om datan har lästs in korrekt.

**Steg 2: Ladda upp bildfiler**

1.  **Produktbilder**: Se till att dina produktbilders filnamn exakt matchar `sku` i din Excel-fil (t.ex. `2327.jpg`).
2.  **Ursprungsflaggor (Valfritt)**: Om du använder `origin`-kolumnen, se till att dina flaggbilders filnamn matchar landets namn (t.ex. `Thailand.png`, `Vietnam.png`).
3.  Klicka på **Välj filer (Choose Files)** under "Steg 2: Ladda upp produktbilder" och välj alla dina produktbilder.
4.  För att ladda upp flaggor, klicka på **Välj filer (Choose Files)** bredvid "Ursprungsflaggor (Origin Flags)" i sektionen "Anpassa utseende" och välj dina flaggbilder.

**Steg 3: Konfigurera katalogläge och titlar**

1.  Ange ett datum eller en allmän titel i fältet **Kampanjdatum (Promotion Date)** (t.ex. "Juli 2025 Special").
2.  Klicka på fliken **Kampanj (Promotion)** eller **Nyheter (New Arrivals)** för att välja katalogens designläge.
3.  Fyll i motsvarande titel för det valda läget (t.ex. "Kampanj" för Promotion, "NYHETER" för New Arrivals).

**Steg 4: Anpassa sidfot**

1.  Klicka i textrutan under **Anpassa sidfotstext (Custom Footer Text)**.
2.  Använd verktygsfältet för att göra texten **Fet**, *Kursiv* eller \<u\>Understruken\</u\>.
3.  Ändra typsnitt, textstorlek och textfärg med hjälp av rullgardinsmenyerna och färgväljaren. Dina ändringar visas i live-förhandsgranskningen.

**Steg 5: Anpassa utseende**
Denna sektion låter dig helt anpassa din katalog till ditt varumärke. För bästa resultat, använd de rekommenderade bildstorlekarna.

  * **Sidhuvud-logotyp (Header Logo)**: Ditt företags logotyp. (Rekommenderat: 400x100 pixlar)
  * **Sidhuvud-bakgrund (Header BG)**: En bakgrund för titelområdet. (Rekommenderat: 600x100 pixlar)
  * **Sidbakgrund (Page BG)**: En bakgrund för hela A4-sidan. (Rekommenderat: 1240x1754 pixlar)
  * **Prislapps-bakgrund (Price Tag BG)**: En anpassad bakgrund för prislappen i Kampanjläget. (Rekommenderat: 100x100 pixlar)
  * **Ursprungsflaggor (Origin Flags)**: Din samling av nationsflaggor.
  * **Sidfots-bild (Footer Image)**: En logotyp eller bild som ska visas i sidfoten. (Rekommenderat: 100x100 pixlar)

**Steg 6: Förhandsgranska och Exportera**

1.  Använd reglaget och knapparna (`+` / `-`) för **Zooma förhandsgranskning (Zoom Preview)** för att inspektera katalogsidorna noggrant.
2.  Kontrollera **statuspanelen** längst ner på kontrollpanelen för eventuella felmeddelanden, som t.ex. saknade bilder.
3.  När du är nöjd, klicka på knappen **Skriv ut eller spara som PDF (Print or Save as PDF)**.
4.  I webbläsarens utskriftsdialog, välj din skrivare eller välj **"Spara som PDF"** som destination för att få en digital fil.
