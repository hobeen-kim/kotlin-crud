# kotlin 으로 간단한 CRUD 게시판 실습입니다.

# 기능
- JWT 활용 로그인
- 게시글 CRUD
- 게시글 추천 기능
- 게시글 추천, 조회, 최신순 페이징 정렬
- 댓글 CRUD

- **미구현 : 프론트 페이지**

# 사용 기술
- Kotlin, SpringBoot 3.0
- Spring Security
- Spring Data JPA
- H2 InmemoryDB

# API
|URL|Method|기능|
|---|------|----|
|/posts?page=xx&sort=xx  |GET|포스트 목록 조회|
|/posts/{post-id}|GET|포스트 단건 조회|
|/posts|POST|포스트 생성|
|/posts/{post-id}|PATCH|포스트 수정|
|/posts/{post-id}|DELETE|포스트 삭제|
|/posts/{post-id}/upvote|PUT|추천 기능|
|/replies?page=x|GET|댓글 목록 조회|
|/replies/{reply-id}|GET|댓글 단건 조회|
|/replies|POST|댓글 생성|
|/replies/{reply-id}|PATCH|댓글 수정|
|/replies/{reply-id}|DELETE|댓글 삭제|
