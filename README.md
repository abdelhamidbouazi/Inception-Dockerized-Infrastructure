# Inception

**Inception** is a system administration and DevOps-focused project at **42/1337 School**, designed to introduce students to containerization and orchestration using Docker, Docker Compose, and other DevOps tools. This project aims to teach students how to set up and manage multiple containers to deploy a functional web application infrastructure efficiently.

---

## Project Overview

The project involves creating a complete web infrastructure by orchestrating multiple Docker containers. The setup includes services such as Nginx, MariaDB, WordPress, and Redis, to provide a comprehensive understanding of Docker container management, networking, and resource optimization.

---

## Key Features

- **Docker Containers**: Efficiently containerize multiple services to isolate and manage resources.
- **Docker Compose**: Utilize Docker Compose to simplify multi-container management and orchestration.
- **Nginx as Reverse Proxy**: Configure Nginx to act as a reverse proxy, enhancing security and performance.
- **Database Management**: Set up and configure MariaDB for persistent data storage.
- **Caching with Redis**: Implement Redis caching for improved application responsiveness and reduced database load.
- **SSL/TLS Security**: Secure the application with SSL/TLS certificates.

---

## Requirements

- **Operating System**: Linux/MacOS
- **Tools**: Docker, Docker Compose

---

## Installation

1. **Clone the repository:**

   ```shell
   git clone https://github.com/yourusername/inception.git
   cd inception
   ```

2. **Start the infrastructure:**

   ```shell
   docker-compose up --build
   ```

---

## Project Structure

```
inception/
├── docker-compose.yml
├── srcs/
│   ├── nginx/
│   │   ├── Dockerfile
│   │   └── conf/nginx.conf
│   ├── wordpress/
│   │   └── Dockerfile
│   ├── mariadb/
│   │   ├── Dockerfile
│   │   └── conf/my.cnf
│   └── redis/
│       └── Dockerfile
└── .env
```

---

## Configuration (.env file)

The `.env` file should contain environment variables needed to configure services securely and efficiently:

```
DOMAIN_NAME=abouazi.42.fr
DB_NAME=wordpress
DB_USER=user
DB_PASSWORD=password
DB_ROOT_PASSWORD=rootpassword
```

---

## Accessing the Application

After deployment, access your web application via:

```
https://abouazi.42.fr
```

---

## Useful Commands

- **Stop all containers:**

  ```shell
  docker-compose down
  ```

- **Check container status:**

  ```shell
  docker-compose ps
  ```

---

## Resources for Studying

- [Docker Documentation](https://docs.docker.com/)
- [Docker Compose Documentation](https://docs.docker.com/compose/)
- [Official Nginx Documentation](https://nginx.org/en/docs/)
- [MariaDB Documentation](https://mariadb.com/kb/en/documentation/)
- [WordPress Documentation](https://wordpress.org/support/)
- [Redis Documentation](https://redis.io/docs/)

---

## References

- [42/1337 School Project Guidelines](https://projects.intra.42.fr/inception/mine)

---

## Credits

Project developed by [abouazi](https://profile.intra.42.fr/users/abouazi) at [42/1337 School](https://1337.ma/).

---

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) file for details.
