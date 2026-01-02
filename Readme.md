# Lobsters Feed for TRMNL

Display the latest stories from [Lobste.rs](https://lobste.rs) on your TRMNL e-ink device.

Lobsters is a computing-focused community centered around link aggregation and discussion, maintained by a culture that values thoughtful, on-topic conversation.

<img width="1660" height="998" alt="image" src="https://github.com/user-attachments/assets/14ddd243-29da-4336-b8eb-995071f6c317" />

## Setup

### 1. Install the Plugin

Install from the [TRMNL Plugin Directory](https://usetrmnl.com/recipes) or add manually to your device.

### 2. Configure

Choose your preferred feed type:
- **Hottest**: Most popular and actively discussed stories
- **Newest**: Latest submissions to Lobsters

## Views

| View | File | Description |
|------|------|-------------|
| Full | `full.liquid` | Full screen display |
| Half Horizontal | `half_horizontal.liquid` | Half screen, landscape |
| Half Vertical | `half_vertical.liquid` | Half screen, portrait |
| Quadrant | `quadrant.liquid` | Quarter screen |

## Local Development

Edit `.trmnlp.yml` and set your preferences:
```yaml
custom_fields:
  feed_type: "hottest"
```

Run the development server:
```bash
docker run \
  --publish 8001:4567 \
  --volume "$(pwd):/plugin" \
  trmnl/trmnlp serve
```

## Links

* [Lobste.rs](https://lobste.rs) - The Lobsters community
* [Lobsters About Page](https://lobste.rs/about) - Learn more about the community

## Support

If you find this plugin useful, consider supporting my work: [r1l.in/s](https://r1l.in/s)

Need a custom TRMNL plugin for your business? I'm available for contract work. Reach out at [hello@rishikeshs.com](mailto:hello@rishikeshs.com).

## License

MIT
