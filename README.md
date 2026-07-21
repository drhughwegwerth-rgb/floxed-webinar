# Antibiotic Damage Webinar Landing Page

Static webinar landing page prepared for deployment through GitHub and Coolify.

## Coolify configuration

- Build pack: Dockerfile
- Dockerfile location: `/Dockerfile`
- Exposed port: `80`
- Health check path: `/`
- Domain: configure the final Hostinger-managed hostname in Coolify

## Hostinger DNS

After Coolify supplies the destination hostname or server IP, create the matching DNS record in Hostinger and add the same domain to the Coolify resource. Enable HTTPS in Coolify after DNS resolves.

## Local Docker preview

```sh
docker build -t webinar-landing-page .
docker run --rm -p 8080:80 webinar-landing-page
```

Then open `http://localhost:8080`.
