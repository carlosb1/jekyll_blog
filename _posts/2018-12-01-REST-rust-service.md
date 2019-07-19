---
layout: post
title: REST API Service in Rust
categories: rust
---
### REST Service in Rust

I started a boilerplate project for future web implementations in Rust. As far as I know the normal backend is Rocket + Diesel. With this project I will be able to extend the boilerplate for future requirements, and if it is necessary include any type.

It is a minimal example for a REST API service.

- `db.rs` Database manager class
- `error.rs` Class to manage error messages
- `main.rs` Entry point which includes REST service
- `schema.rs` Schema definition to connect with the database Postgres

Original [source code](https://github.com/carlosb1/examples-rust/tree/master/my_rocket_diesel_demo)
