# Notification Images

This folder contains the image used for push notifications.

## Current Setup

- `notification.png` - Single image used for all notification types (currently the app launcher icon)

## Image URL

Once deployed to GitHub Pages, the image will be accessible at:
```
https://marpau0755.github.io/tophundred-privacy/images/notification.png
```

## Cloud Functions Configuration

The Cloud Functions are already configured to use this image. The URL is set in `cloud_functions_notifications.js`:
```javascript
const NOTIFICATION_IMAGE_URL = 'https://marpau0755.github.io/tophundred-privacy/images/notification.png';
```

## Future: Custom Images

If you want to use different images for different notification types later, you can:
1. Add new images here (e.g., `achievement.png`, `power-full.png`, `streak.png`)
2. Update the `NOTIFICATION_IMAGES` object in Cloud Functions
3. Reference specific images in each notification type

