# README

## Project Overview

This project models a simple social media platform using SQL. It includes tables for users, posts, comments, likes, and followers, allowing for basic interactions like posting, commenting, liking, and following.

---

## Database Tables

1. **users**: Stores user info (`user_id`, `name`, `email`, `phone`).
2. **posts**: Contains posts made by users with fields for `post_id`, `user_id`, `caption`, `image_url`, and `created_time`.
3. **comment**: Holds comments on posts, with `comment_id`, `post_id`, `user_id`, `comment_text`, and `created_at`.
4. **likes**: Tracks likes on posts with `like_id`, `post_id`, `user_id`, `like_count`, and `created_at`.
5. **followers**: Manages user follow relationships using `follower_id`, `user_id`, `follower_user_id`, and `created_at`.

---

## Sample Data

Sample data is provided for all tables, including users like 'John Smith' and 'Jane Doe', along with their posts, comments, likes, and follower relationships.

---

## Key Queries

- **Update Post Caption**: Update the caption for `post_id = 4`.
  
  ```sql
  UPDATE posts SET caption = 'Vaccation pictures' WHERE post_id = 4;
