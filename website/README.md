# XOLERIC AI Operating System

The world's first AI-native operating system with custom Rust microkernel and integrated AI inference.

## Features

- **Custom Rust Microkernel** - 27KB minimal kernel with memory safety
- **Integrated AI Core** - XAI daemon with 4 pre-installed models
- **Smart Package Manager** - xpkg with AI dependency resolution
- **Intelligent Init System** - xinit with self-healing capabilities
- **AI-Enhanced Security** - Kernel modules with anomaly detection
- **Optimized Performance** - 8.9x faster inference with model warm-up

## Quick Start

```bash
# Write to USB
sudo dd if=xoleric-pc-v1.0.0.iso of=/dev/sdX bs=4M

# Boot from USB
# Select XOLERIC from GRUB menu

# Use AI
curl http://localhost:11434/api/chat -d '{"model":"tinyllama","messages":[{"role":"user","content":"Hello!"}]}'
```

## Performance

| Model | Response Time | Use Case |
|-------|---------------|-----------|
| tinyllama | 3s | Fast queries ⭐ |
| phi | 9s | General purpose |
| xai-fast | 21s | Optimized |
| llama3.2:3b | 187s (cold) | Complex reasoning |

## Documentation

See [docs.xoleric.ai](https://xolerc.github.io/xoleric/) for full documentation.

## License

MIT License

## Support

- GitHub Issues: https://github.com/xolerc/xoleric/issues
- Documentation: https://xolerc.github.io/xoleric/
