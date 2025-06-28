# My Profile - Portfolio Website

## Cài đặt và chạy locally

1. Cài đặt NodeJS (nếu chưa có)
2. Clone repository và chạy:
   ```bash
   npm install
   npm start
   ```

## Build cho production
```bash
npm run build
```

## Deploy lên Vercel

### Cách 1: Deploy qua Vercel CLI
1. Cài đặt Vercel CLI:
   ```bash
   npm i -g vercel
   ```

2. Login vào Vercel:
   ```bash
   vercel login
   ```

3. Deploy:
   ```bash
   vercel
   ```

### Cách 2: Deploy qua GitHub
1. Push code lên GitHub
2. Vào [vercel.com](https://vercel.com)
3. Import project từ GitHub
4. Vercel sẽ tự động detect đây là React app và deploy

### Cách 3: Deploy trực tiếp từ folder
1. Vào [vercel.com](https://vercel.com)
2. Click "New Project"
3. Upload folder project
4. Vercel sẽ tự động build và deploy

## Cấu hình
- File `vercel.json` đã được tạo để cấu hình routing cho SPA
- Homepage đã được set về "." để tương thích với Vercel
- Build script đã được thêm vào package.json

## Lưu ý
- Vercel sẽ tự động deploy khi có thay đổi trên GitHub (nếu dùng cách 2)
- Mỗi commit sẽ tạo một preview deployment
- Production URL sẽ được cung cấp sau khi deploy thành công
