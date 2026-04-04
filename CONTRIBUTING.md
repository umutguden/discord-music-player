# Contributing

Contributions are welcome. This document provides guidelines for contributing to this project.

## Reporting Bugs

1. Check existing [issues](https://github.com/hmddevs/discord-music-player/issues) to avoid duplicates.
2. Use a clear, descriptive title.
3. Include steps to reproduce the issue.
4. Describe expected versus actual behaviour.
5. Include your Node.js version and operating system.

## Suggesting Features

Open an issue with the `enhancement` label. Describe the feature, its use case, and how it would benefit users.

## Pull Requests

1. Fork the repository.
2. Clone your fork locally.
3. Create a feature branch: `git checkout -b feature/your-feature`.
4. Make your changes and test locally.
5. Commit with clear messages: `git commit -m 'Add: brief description'`.
6. Push to your fork: `git push origin feature/your-feature`.
7. Open a pull request against `main`.

## Code Style

- Use consistent indentation (2 spaces).
- Follow existing code patterns.
- Add comments for complex logic.
- Keep functions focused and small.

## Adding New Commands

1. Create a new file in `commands/`.
2. Export `config` with `name` and `aliases`.
3. Export an `hmd` async function with `(client, message, args, config)`.
4. Follow existing command patterns for consistency.

```js
const { MessageEmbed } = require('discord.js');

module.exports.config = {
    name: 'mycommand',
    aliases: ['mc', 'myc']
};

module.exports.hmd = async (client, message, args, config) => {
    // Your command logic here
};
```

## Questions

Open an issue for any questions or discussion.
