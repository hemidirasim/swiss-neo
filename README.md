# Swissneo Baby Nutrition Website

Swissneo baby nutrition website with admin panel and multilingual support.

## 🚀 Vercel Deployment

### 1. Environment Variables Setup

Vercel dashboard-da bu environment variable-ı əlavə edin:

```
BLOB_READ_WRITE_TOKEN=vercel_blob_rw_lpXh5J5CALn3pKRK_Vx0SPIGeZbAkiuiyC9UyRvbW0EwIGk
```

**Addım-addım:**
1. Vercel dashboard-a daxil olun
2. Proyektinizi seçin
3. "Settings" tab-ına keçin
4. "Environment Variables" bölməsini tapın
5. "Add New" düyməsinə basın
6. Name: `BLOB_READ_WRITE_TOKEN`
7. Value: `vercel_blob_rw_lpXh5J5CALn3pKRK_Vx0SPIGeZbAkiuiyC9UyRvbW0EwIGk`
8. Environment: Production, Preview, Development (hamısını seçin)
9. "Save" düyməsinə basın

### 2. Deploy

```bash
# Vercel CLI ilə
vercel --prod

# Və ya GitHub-dan avtomatik deploy
```

## 🛠️ Local Development

### Installation

```bash
npm install
```

### Development Server

```bash
npm run dev
```

### Build

```bash
npm run build
```

### Preview

```bash
npm run preview
```

## 🔐 Admin Panel

- **URL**: `/swissadmin`
- **Username**: `admin`
- **Password**: `swissneo2024`
- **Session**: 7 gün avtomatik uzadılır

## 📝 Features

- ✅ Multilingual support (AZ/EN)
- ✅ Admin panel with session management
- ✅ Article management with beautiful image uploader
- ✅ Contact form submissions
- ✅ Responsive design
- ✅ LocalStorage for data persistence

## 🎨 Qəşəng Visual Uploader

### Modern Şəkil Yükləmə Sistemi
- ✅ **Drag & Drop** funksiyası
- ✅ **Visual feedback** və animasiyalar
- ✅ **Hover effects** və transitions
- ✅ **Loading states** və progress
- ✅ **File validation** (format və ölçü)
- ✅ **Preview** funksiyası
- ✅ **Remove** və **Replace** düymələri
- ✅ **Responsive design**
- ✅ **Vercel Blob Storage** inteqrasiyası
- ✅ **Image compression** və optimization
- ✅ **Multi-level fallback** sistemi

### Xüsusiyyətlər:
- 🎯 **Drag & Drop** - Şəkli sürükləyib buraxın
- 🖱️ **Click to Upload** - Klikləyərək şəkil seçin
- 👁️ **Live Preview** - Dərhal preview görün
- ✨ **Smooth Animations** - Gözəl animasiyalar
- 🔄 **Replace Image** - Mövcud şəkli dəyişdirin
- 🗑️ **Remove Image** - Şəkli silin
- 📱 **Mobile Friendly** - Mobil cihazlarda işləyir
- ☁️ **Cloud Storage** - Vercel Blob Storage-a yüklənir
- 🔄 **Fallback System** - Vercel uğursuz olsa base64 istifadə edir
- 📏 **Auto Compression** - Böyük şəkillər avtomatik sıxılır

### Dəstəklənən Formatlar:
- ✅ **PNG** - Rəqəmsal şəkillər
- ✅ **JPG/JPEG** - Fotoşəkillər
- ✅ **GIF** - Animasiyalı şəkillər
- ✅ **WebP** - Modern format

### Ölçü Limiti:
- 📏 **Maksimum 10MB** fayl ölçüsü
- ⚡ **Avtomatik sıxılma** 5MB-dan çox fayllar üçün
- ☁️ **Vercel Blob Storage** ilə saxlanılır
- 💾 **Base64 fallback** sistem

### API Endpoint:
- 🔗 **`/api/upload-image`** - Şəkil yükləmə endpoint-i
- 📤 **FormData** ilə şəkil göndərilir
- ☁️ **Vercel Blob Storage**-a yüklənir
- 🔗 **Public URL** qaytarılır
- 🔄 **Fallback** base64 encoding

### Şəkil Yükləmə Prosesi:
1. **Şəkil seçilir** visual uploader ilə
2. **Validation** keçir (format və ölçü)
3. **Compression** (5MB-dan çox fayllar üçün)
4. **Vercel Blob Storage**-a yükləmə cəhdi
5. **Uğurlu olsa** - Vercel Blob URL qaytarılır
6. **Uğursuz olsa** - Base64 encoding istifadə edilir
7. **Məqalə ilə birlikdə** saxlanılır

### Data Persistence:
- 💾 **localStorage** ilə məqalələr saxlanılır
- 🔄 **Singleton pattern** - Tək instance
- 📊 **Console logging** - Debug üçün
- 🛡️ **Error handling** - Fallback sistemlər

### ImageService Xüsusiyyətləri:
- 🔍 **File validation** - Format və ölçü yoxlaması
- 📐 **Dimension detection** - Şəkil ölçülərini tapır
- 🗜️ **Auto compression** - Böyük şəkilləri sıxır
- ☁️ **Vercel Blob upload** - Etibarlı cloud storage
- 💾 **Base64 fallback** - Offline dəstəyi
- 🛡️ **Error handling** - Bütün xətalar tutulur

### Environment Variables:
```
BLOB_READ_WRITE_TOKEN=vercel_blob_rw_lpXh5J5CALn3pKRK_Vx0SPIGeZbAkiuiyC9UyRvbW0EwIGk
```

## 🏗️ Project Structure

```
src/
├── components/          # UI components
│   ├── ui/             # Shadcn/ui components
│   └── ImageUploader.tsx # Beautiful image uploader
├── contexts/           # React contexts
├── data/              # Static data
├── hooks/             # Custom hooks
├── pages/             # Page components
├── services/          # API services
└── types/             # TypeScript types
```

## 🔧 Configuration

### Vite Config
- Build optimization
- Vercel deployment ready
- SPA routing support

### Vercel Config
- SPA fallback routing
- Static asset caching

## 🚨 Troubleshooting

### Vercel Deployment Issues
1. Environment variables düzgün qurulub
2. Build logs-ı yoxlayın
3. Vercel logs-ı yoxlayın
4. Local build test edin

### Local Development Issues
1. Node.js versiyası 18+ olmalıdır
2. npm install tamamlanmalıdır
3. Port 8080 boş olmalıdır
4. Browser console xətalarını yoxlayın
