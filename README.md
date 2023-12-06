
# redis-rust

This repository contains examples of how to use Rust to interact with Redis, utilizing the `redis-rs` client. It demonstrates the implementation of various Redis data structures and commands, including Strings, Hashes, Lists, Sets, and Sorted Sets. The code showcases both high and low-level Redis client API usage.

## Prerequisites

- Rust (version 1.39 or higher)
- A Redis instance (either a local setup using Docker or a service like Azure Cache for Redis)

To set up a Redis instance using Docker:

```bash
docker run --rm -p 6379:6379 redis
```

## Connecting to Redis

The `connect` function establishes a connection to Redis using environment variables `REDIS_HOSTNAME` and `REDIS_PASSWORD`. For TLS-enabled connections, like Azure Cache for Redis, set the `IS_TLS` environment variable.

## Basic Operations on Strings and Integers

Examples include using SET, GET, and INCR commands for string and integer manipulation.

## Working with Hash Data Structures

Demonstrates storing and retrieving data using Redis HASH, including both low-level commands and high-level APIs.

## Using Redis Lists

Showcases list operations like LPUSH, LPOP, and LRANGE.

## Managing Data in Redis Sets

Covers set operations, including adding elements and checking membership.

## Utilizing Redis Sorted Sets

Demonstrates adding elements to sorted sets and retrieving them with scores.

## Running the Application

Clone the repository and navigate to the directory:

```bash
git clone https://github.com/abhirockzz/rust-redis-101.git
cd rust-redis-101
```

Set up the necessary environment variables based on your Redis setup and run the application using Cargo:

```bash
export REDIS_HOSTNAME=localhost:6379 # or your Redis instance details
cargo run
```

Explore the examples and learn about various Redis operations in Rust.
