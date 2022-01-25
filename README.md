# offtheback.in
[![Netlify Status](https://api.netlify.com/api/v1/badges/dd1d86c5-dc6f-4890-a14c-337abaf099e0/deploy-status)](https://app.netlify.com/sites/off-the-back/deploys)


# Converting PNG and JPG photos to WebP
find ./ -type f -name '*.png' -exec sh -c 'avifenc --min 10 --max 30 $1 "${1%.png}.avif"' _ {} \;  
find ./ -type f -name '*.jpg' -exec sh -c 'cwebp $1 -o "${1%.jpg}.webp"' _ {} \;  

via [WebP and AVIF images on a Hugo website](https://pawelgrzybek.com/webp-and-avif-images-on-a-hugo-website/)
