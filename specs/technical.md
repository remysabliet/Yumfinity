# Technical Specification

## Technical Stack

- **Frontend: Next.js** - A React framework for building JavaScript applications. It supports server-side rendering and generating static websites, which is great for performance and SEO. It also has a great developer experience with features like hot module replacement.

- **Backend: Next.js API Routes with GraphQL** - Next.js API routes provide a solution to build your API with Next.js and Node.js. GraphQL will be used as the query language for your API, allowing clients to fetch exactly the data they need.

- **Database: PostgreSQL on AWS RDS** -  A powerful, open source object-relational database system with over 30 years of active development that has earned it a strong reputation for reliability, feature robustness, and performance. AWS RDS makes it easy to manage your PostgreSQL instances.

- **Authentication: Next-Auth** - A complete full-stack authentication solution for Next.js applications. It is designed from the ground up to support Next.js and Serverless.

- **Search Functionality: Elasticsearch** - A distributed, RESTful search and analytics engine capable of addressing a growing number of use cases. As the heart of the Elastic Stack, it centrally stores your data for lightning fast search, fine‑tuned relevancy, and powerful analytics that scale with ease.

- **Infrastructure: AWS** - Amazon Web Services offers reliable, scalable, and inexpensive cloud computing services. You can use services like AWS Amplify for hosting your Next.js application, AWS Aurora for your PostgreSQL database.

- **Storage: AWS S3** - For storing any static files (video, images, voice recording) or images related to your application. 

- **CDN: AWS CloudFront.** - Faster delivery of static assets

- **APIs** -: GraphQL with Apollo Server - GraphQL is a query language for APIs and a runtime for executing those queries with your existing data. Apollo Server is an open-source, spec-compliant GraphQL server that's compatible with any GraphQL schema.

- **Image Handling** - Next.js has built-in support for image optimization, which can be used to serve optimized, resized, and transformed images to your users. Images can be stored in AWS S3 and served using the AWS CloudFront CDN for faster delivery.

- **Video and audio files**