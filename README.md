# Labyrinth Drift

A simple **world exploration** game built with the **Unity 3D** engine. Control a 3D avatar and explore a **procedurally generated maze** with walls, rooms, doors, trees, stairs, and more. The maze is never the same twice and expands as you explore—reaching the edge triggers generation of new content for an effectively endless world.

![Image of Labyrinth Drift](http://cdn.rawgit.com/erikbuck/MazeVenture/master/MazeVenture.png)

---

## Features

- **Procedural maze generation** — Each playthrough produces a unique layout
- **Multi-level mazes** — Stairs connect different elevations with landings and railings
- **Rooms and doors** — Connected spaces with configurable door probability
- **Decorations** — Trees, wall variants, columns, and banisters
- **Smooth player movement** — Grid-based movement with walk/run and directional facing
- **Third-person view** — Camera follows the player through the maze

---

## Technology

- **Engine:** Unity 3D
- **Language:** C#
- **Content:** Custom 3D models and scripts plus free assets from the Unity Asset Store (e.g. Yurowm character/animations, SpeedTree-style trees)

---

## Getting Started

### Requirements

- **Unity** (version compatible with the project; typically Unity 5.x or later for this codebase)

### Running the Project

1. Clone or download this repository.
2. Open the project folder in **Unity Hub** or Unity (Open Project → select the project root).
3. Open the main scene: `Assets/Scene.unity`.
4. Press **Play** in the Unity Editor.

### Controls

| Key | Action |
|-----|--------|
| **W** / **↑** | Move forward |
| **S** / **↓** | Move backward |
| **A** / **←** | Move / turn left |
| **D** / **→** | Move / turn right |
| **Q** | Turn left (in place) |
| **E** | Turn right (in place) |
| **Space** | Restart game (new maze) |

The player automatically walks or runs depending on distance to the next cell. Movement is grid-based: one keypress advances one cell in the chosen direction.

---

## Project Structure

```
LabyrinthDrift/
├── Assets/
│   ├── Scene.unity              # Main game scene
│   ├── Scripts/                # Core C# game logic
│   │   ├── GameManager.cs      # Maze + player setup, restart
│   │   ├── Player.cs          # Movement, routing, input
│   │   ├── Maze.cs            # Procedural generation
│   │   ├── MazeCell.cs        # Cell data and edges
│   │   ├── MazePassage.cs     # Open passages
│   │   ├── MazeDoor.cs        # Doors between rooms
│   │   ├── MazeStairs.cs      # Stairs and landings
│   │   ├── MazeWall.cs        # Walls and railings
│   │   ├── MazeDirection.cs   # Cardinal directions
│   │   ├── IntVector2.cs     # 2D integer coordinates
│   │   └── ...
│   ├── Prefabs/               # Maze and player prefabs
│   ├── Materials/             # Wall, floor, door materials
│   ├── Yurowm/                # Character & animations (Asset Store)
│   └── Free_SpeedTrees/       # Tree assets
├── LICENSE.md
└── README.md
```

---

## License

Redistribution and use in source and binary forms, with or without modification, are permitted under the terms in LICENSE.md.

---

*Labyrinth Drift — endless mazes, one play at a time.*

- Fix the encoding issue when reading config files with non-ASCII

- Clean up the TODO comments that were already addressed

- Correct the default so it matches what the documentation says

- Handle timeout gracefully and return a clear error to the caller

- Bump the dependency to fix the compatibility issue with Python 3.12

- Update the example config with all available options and comments

- Improve the default config so it works out of the box for dev

- Improve performance by caching the result of the expensive lookup

- Update README with installation steps and environment variable documentation

- Bump the version and tag the release in the repo

- Handle connection reset by the peer without crashing the worker

- Handle timeout gracefully and return a clear error to the caller

- Support optional config file path via env var for easier deployment

- Correct the formula used for calculating the backoff delay

- Fix the memory leak in the long-running worker process

- Support passing secrets via a separate file for security

- Update README with installation steps and environment variable documentation

- Support optional config file path via env var for easier deployment

- Fix the off-by-one error in the date range iterator

- Clean up leftover code from the previous implementation

- Improve error message when the required env var is not set

- Implement a simple metrics endpoint for Prometheus scraping

- Clean up the test fixtures and move shared data to a single file

- Bump minimum Python version to 3.10 and update type hints accordingly

- Handle the redirect response and follow it to get the final resource

- Improve the default config so it works out of the box for dev

- Simplify the CLI by merging the two similar subcommands into one

- Clean up leftover code from the previous implementation

- Improve the default config so it works out of the box for dev

- Handle the case when the config file exists but is not readable

- Remove the feature flag now that the feature is fully rolled out

- Bump the CI image to use the latest stable runner version

- Adjust the threshold so we only log when it's actually an issue

- Support custom headers in the client for API key or auth tokens

- Refactor the data layer to separate read and write paths

- Clean up leftover code from the previous implementation

- Refactor the parser to use a proper state machine instead of regex

- Correct the default so it matches what the documentation says

- Adjust timeout and retry settings based on production observations

- Implement a small in-memory cache for the config to avoid re-reading

- Correct the formula used for calculating the backoff delay

- Fix the ordering of middleware so auth runs before the handler

- Implement request ID propagation for better tracing across services

- Update dependencies and resolve compatibility warning from pytest

- Refactor the helper to accept an optional callback for progress

- Simplify the main loop by extracting request handling into a dedicated function

- Simplify the CLI by merging the two similar subcommands into one

- Implement fallback to default value when config key is missing

- Clean up the TODO comments that were already addressed

- Bump the CI image to use the latest stable runner version

- Remove hardcoded credentials and move to env-based configuration

- Refactor config loading into a separate module for better testability

- Fix the encoding issue when reading config files with non-ASCII

- Add a note in the README about the breaking change in 2.0

- Handle the redirect response and follow it to get the final resource

- Correct typo in the error message shown when validation fails

- Fix the off-by-one error in the date range iterator

- Bump version to 1.2.0 and add changelog entry for the new features

- Implement proper backoff with jitter for the retry logic

- Adjust log level for noisy messages that were filling the logs

- Add a smoke test that runs in CI to catch obvious regressions

- Clean up the TODO comments that were already addressed

- Add integration test that covers the full flow from request to response

- Simplify the main loop by extracting request handling into a dedicated function

- Implement retry logic for the API client when the remote returns 5xx

- Fix the encoding issue when reading config files with non-ASCII

- Remove the feature flag now that the feature is fully rolled out

- Add integration tests for the new export endpoint

- Support custom headers in the client for API key or auth tokens

- Handle the redirect response and follow it to get the final resource

- Bump minimum Python version to 3.10 and update type hints accordingly

- Refactor error handling to use a custom exception hierarchy

- Refactor the helper to accept an optional callback for progress

- Correct the default path used when no config file is specified

- Support config reload without restart via SIGHUP or file watch

- Remove the experimental feature that didn't make it into the release

- Clean up duplicate logic between the sync and async code paths

- Correct typo in the error message shown when validation fails

- Fix race condition in the cache that could return stale data under load

- Refactor the data layer to separate read and write paths

- Clean up the deprecated alias and point callers to the new name

- Add a smoke test that runs in CI to catch obvious regressions

- Improve the startup time by lazy-loading the heavy modules

- Add a comment explaining why we disable the linter on this line

- Implement a simple health check endpoint for the load balancer

- Implement proper backoff with jitter for the retry logic

- Handle edge case when the response body is empty but status is 200

- Simplify the config merge logic so overrides are predictable

- Simplify the auth flow by using a single token source

- Refactor utils to use a single source of truth for default values

- Implement request ID propagation for better tracing across services

- Refactor the parser to use a proper state machine instead of regex

- Simplify the CLI by merging the two similar subcommands into one

- Refactor the parser to use a proper state machine instead of regex

- Correct the docstring to match the actual behavior of the function

- Add integration test that covers the full flow from request to response

- Refactor utils to use a single source of truth for default values

- Clean up the TODO comments that were already addressed

- Adjust the threshold so we only log when it's actually an issue

- Support optional config file path via env var for easier deployment

- Adjust the pool size to match the actual concurrency we need

- Implement fallback to default value when config key is missing

- Clean up the test fixtures and move shared data to a single file

- Update the deployment docs with the new environment variables

- Simplify the config merge logic so overrides are predictable

- Improve the startup time by lazy-loading the heavy modules

- Support environment-specific overrides via separate config files

- Add integration test that covers the full flow from request to response

- Improve the CLI help text so it's clear how to use each option

- Adjust default timeout value to prevent premature connection drops

- Add integration tests for the new export endpoint

- Fix race condition in the cache that could return stale data under load

- Add a small delay between retries to avoid thundering herd

- Correct typo in the error message shown when validation fails

- Simplify the CLI by merging the two similar subcommands into one

- Adjust the threshold so we only log when it's actually an issue

- Add a unit test for the edge case when the list is empty

- Refactor the data layer to separate read and write paths

- Clean up the TODO comments that were already addressed

- Simplify the config validation by using a declarative schema

- Clean up unused imports and fix formatting to match the project style guide

- Remove the temporary debug endpoint before the release

- Update the changelog with the fixes included in this release

- Support custom headers in the client for API key or auth tokens

- Remove the temporary debug endpoint before the release

- Implement retry logic for the API client when the remote returns 5xx

- Handle missing optional field in the response without raising

- Improve test coverage for the helpers module to above 90%

- Support environment-specific overrides via separate config files

- Simplify the auth flow by using a single token source

- Correct the comparison that was using the wrong operator

- Correct the docstring to match the actual behavior of the function

- Improve the error recovery when the database connection is lost

- Clean up the commented-out code that was left from debugging

- Simplify the CLI by merging the two similar subcommands into one

- Simplify the config merge logic so overrides are predictable

- Fix the ordering of middleware so auth runs before the handler

- Update the deployment docs with the new environment variables

- Remove the feature flag now that the feature is fully rolled out

- Implement a simple health check endpoint for the load balancer

- Remove obsolete workaround now that the upstream bug is fixed

- Implement proper backoff with jitter for the retry logic

- Correct the default so it matches what the documentation says

- Remove deprecated CLI flag and update docs to use the new option

- Clean up leftover code from the previous implementation

- Update documentation to reflect the new API and usage examples

- Refactor the client to use async context manager for the session

- Support both relative and absolute paths for the config file

- Adjust the batch size to reduce memory usage on large inputs

- Refactor exports so the public API is clearer and easier to use

- Adjust default timeout value to prevent premature connection drops

- Improve the CLI help text so it's clear how to use each option

- Support passing secrets via a separate file for security

- Add a unit test for the edge case when the list is empty

- Support both YAML and JSON config formats for flexibility

- Support config reload without restart via SIGHUP or file watch

- Handle the duplicate key case by merging the values instead of failing

- Support custom headers in the client for API key or auth tokens

- Simplify the main loop by extracting request handling into a dedicated function

- Implement proper backoff with jitter for the retry logic

- Add a smoke test that runs in CI to catch obvious regressions

- Add integration test that covers the full flow from request to response

- Adjust default timeout value to prevent premature connection drops

- Add a comment explaining why we disable the linter on this line

- Simplify the auth flow by using a single token source

- Improve the default config so it works out of the box for dev

- Fix bug where the parser would hang on malformed input

- Fix the memory leak in the long-running worker process

- Bump minimum Python version to 3.10 and update type hints accordingly

- Support passing options through the config file as well as CLI

- Bump dependency to get the security fix for the reported CVE

- Improve test coverage for the helpers module to above 90%

- Correct the docstring to match the actual behavior of the function

- Add a note in the README about the breaking change in 2.0

- Improve logging so we can trace requests through the pipeline in production

- Remove the experimental feature that didn't make it into the release

- Correct the timestamp format to use ISO 8601 for consistency

- Remove hardcoded credentials and move to env-based configuration

- Correct the timestamp format to use ISO 8601 for consistency

- Handle connection reset by the peer without crashing the worker

- Simplify the dependency injection so it's easier to mock in tests

- Adjust the queue size to prevent drops under burst traffic

- Implement a simple metrics endpoint for Prometheus scraping

- Remove obsolete workaround now that the upstream bug is fixed

- Fix the off-by-one error in the date range iterator

- Implement a simple health check endpoint for the load balancer

- Clean up debug print statements before the release

- Handle the case when the external service returns an empty list

- Simplify the auth flow by using a single token source

- Improve the startup time by lazy-loading the heavy modules

- Update documentation to reflect the new API and usage examples

- Implement a simple health check endpoint for the load balancer

- Support passing options through the config file as well as CLI

- Adjust buffer size for the stream reader to reduce memory usage

- Remove obsolete workaround now that the upstream bug is fixed

- Refactor utils to use a single source of truth for default values

- Implement request ID propagation for better tracing across services

- Update the contributing guide with the new review process

- Support passing secrets via a separate file for security

- Remove the temporary debug endpoint before the release

- Handle the duplicate key case by merging the values instead of failing
