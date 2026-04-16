# 🍧 Taste Lab : Back-End Repository

- 편의점, 프렌차이즈 음식점 등 **음식 커스텀 꿀조합을 추천해주는 서비스**

![image](https://github.com/jjunhyeon/algorithm/assets/37209763/2e4bc5b3-bd7d-42c8-b1cc-9c0e21fd3ac2)

---

## 💻 Development Environment

| Composition              | Use                  |
|:-------------------------|:---------------------|
| Project/Issue Management | `Notion`             |
| Knowledge Base           | `Notion`             |
| Source Management        | `GitHub`             |
| IDE / Editor Tools       | `IntelliJ` `dbeaver` |
| Deployment Management    | `GitHub Action`      |

## ⚙️ Tech Stack

| Composition | Use                                                          |
|:------------|:-------------------------------------------------------------|
| API         | `Java11` `SpringBoot`<br/> `SpringSecurity` `JPA` `QueryDSL` |
| DataBase    | `mariaDB`                                                    |
| Build       | `Maven`                                                      |
| Infra       | `Nginx` `NCP` `Docker`                                       |                                       |

---


## 🔗 CI / CD 구성도

```mermaid
flowchart LR
  A[Developer\ngit push] --> B[GitHub Actions\nBuild & Test]
  B --> C[Docker Hub\nImage push]
  C --> D[NCP Server\nDocker pull & run]
  D --> E[Nginx\nReverse proxy]
  D --> F[Spring Boot\n컨테이너]
  F --> G[MariaDB]
```

---

## 📌 주요 기능

- 상품 API (CRUD)

---

## 📎 Link

- [Front Repository](https://github.com/SeoYeonii/yumyum24)
