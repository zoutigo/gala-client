This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.

## Deploy on google

### Connexion o gcloud

`gcloud auth login `

### Set project

`gcloud config set project gala-client xxxxx`

### Create repository

`gcloud artifacts repositories create nextjs-gala-client-repo --repository-format=docker --location=europe-west9 --description="Docker repository gala-client"`

### Lister les repos

`gcloud artifacts repositories list`

### push image

`gcloud builds submit --region=global --tag europe-docker.pkg.dev/gala-client/nextjs-gala-repo/nextjs-gala-client-repo/nextjs-docker-gala-image:tag1`

### deploy

- grab the image name in artficat and paste it
- add the tag at the end

`gcloud run deploy --image=europe-docker.pkg.dev/gala-client/nextjs-gala-repo/nextjs-gala-client-repo/nextjs-docker-gala-image:tag1`
`

## Make Changes and deploy again

### Change the code and save

### Deploy

` gcloud builds submit --region=global --tag europe-docker.pkg.dev/gala-client/nextjs-gala-repo/nextjs-gala-client-repo/nextjs-docker-gala-image:tag1``
 `

### Run the same deploy command

`gcloud run deploy --image=europe-docker.pkg.dev/gala-client/nextjs-gala-repo/nextjs-gala-client-repo/nextjs-docker-gala-image:tag1`
`

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
