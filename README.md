# BoriDrop

BoriDrop is a proof-of-concept file transfer server built with Node.js. It exposes
simple HTTP endpoints for uploading and downloading files. Uploaded files are stored
under the `uploads/` directory.

## Usage

Install dependencies and start the server:

```bash
npm install
npm start
```

Upload a file using `curl`:

```bash
curl -F "file=@/path/to/file" http://localhost:3000/upload
```

Download the file using the filename returned by the upload request:

```bash
curl -O http://localhost:3000/download/<filename>
```

## 개발 계획

전체 플랫폼을 지원하는 파일 전송 앱 개발 계획은 [PLAN.md](PLAN.md) 문서를 참고하십시오.
