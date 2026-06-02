# PDFBolt Postman Collection

<img src="https://img.shields.io/badge/Postman-FF6C37?style=for-the-badge&logo=postman&logoColor=white" height="40" alt="Postman">

A ready-to-fork Postman collection for testing the [PDFBolt API](https://pdfbolt.com). Fork it, add your API key, and start generating PDFs from URLs, HTML, or templates without writing any code.

## Fork the Collection

[<img src="https://run.pstmn.io/button.svg" alt="Run In Postman" width="150">](https://app.getpostman.com/run-collection/40399365-9472b2d4-c8da-4338-8774-962cc6bb9347?action=collection%2Ffork&source=rip_markdown&collection-url=entityId%3D40399365-9472b2d4-c8da-4338-8774-962cc6bb9347%26entityType%3Dcollection%26workspaceId%3D3a6b1d25-d352-4c2e-8a9b-0b4fcb6d6cae#?env%5BPDFBolt%5D=W3sia2V5IjoiYmFzZV91cmwiLCJ2YWx1ZSI6Imh0dHBzOi8vYXBpLnBkZmJvbHQuY29tIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiJodHRwczovL2FwaS5wZGZib2x0LmNvbSIsImNvbXBsZXRlU2Vzc2lvblZhbHVlIjoiaHR0cHM6Ly9hcGkucGRmYm9sdC5jb20iLCJzZXNzaW9uSW5kZXgiOjB9LHsia2V5IjoiQVBJX0tFWSIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6InNlY3JldCIsInNlc3Npb25WYWx1ZSI6IiIsImNvbXBsZXRlU2Vzc2lvblZhbHVlIjoiIiwic2Vzc2lvbkluZGV4IjoxfSx7ImtleSI6IndlYmhvb2tfdXJsIiwidmFsdWUiOiIiLCJlbmFibGVkIjp0cnVlLCJ0eXBlIjoiZGVmYXVsdCIsInNlc3Npb25WYWx1ZSI6IiIsImNvbXBsZXRlU2Vzc2lvblZhbHVlIjoiIiwic2Vzc2lvbkluZGV4IjoyfSx7ImtleSI6ImN1c3RvbVMzX3VybCIsInZhbHVlIjoiIiwiZW5hYmxlZCI6dHJ1ZSwidHlwZSI6ImRlZmF1bHQiLCJzZXNzaW9uVmFsdWUiOiIiLCJjb21wbGV0ZVNlc3Npb25WYWx1ZSI6IiIsInNlc3Npb25JbmRleCI6M31d)

Forking copies the collection and its `PDFBolt` environment into your own Postman workspace.

## Setup

1. **Get your API key.** Find it on the API Keys page in your [PDFBolt dashboard](https://app.pdfbolt.com/register). The free plan includes 100 document conversions per month.
2. **Set the `API_KEY` environment variable** in the forked `PDFBolt` environment. Requests send it as the `API-KEY` header.
3. **(Optional) Set `webhook_url` and `customS3_url`** to test async conversions or uploads to your own S3 bucket. Both are available on paid plans.

## Endpoints

The collection covers all three PDFBolt endpoints:

```text
POST https://api.pdfbolt.com/v1/direct   # returns the binary PDF
POST https://api.pdfbolt.com/v1/sync     # returns JSON with a documentUrl
POST https://api.pdfbolt.com/v1/async    # returns a requestId, delivers the PDF to your webhook
```

## Learn More

- [Postman quick start guide](https://pdfbolt.com/docs/quick-start-guide/postman)
- [Quick start video on YouTube](https://www.youtube.com/watch?v=s9LBZFEYt6g)
- [PDFBolt API documentation](https://pdfbolt.com/docs)
