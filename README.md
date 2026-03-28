# Obsidian Vocabulary Flashcards Plugin

An Obsidian plugin for learning vocabulary through flashcards with LLM-powered pronunciation and definition lookup.

## Features

- **Flashcard View**: Browse vocabulary words with flip-card interaction
- **Search**: Quick search across all vocabulary files
- **Add New Words**: Add words with automatic pronunciation and definition fetching
- **LLM Integration**: Fetch word info from DeepSeek, OpenAI, Anthropic, or custom APIs
- **Duplicate Detection**: Prevents duplicate words and can update definitions for existing entries
- **Mobile Compatible**: Works on Android and iOS

## Installation

### Manual Installation

1. Download `main.js`, `manifest.json`, and `styles.css` from the [Releases](../../releases) page
2. Create a folder named `obsidian-vocabulary-plugin` in your vault's `.obsidian/plugins/` directory
3. Copy the downloaded files into that folder
4. Restart Obsidian and enable the plugin in Settings → Community plugins

## Usage

### Vocabulary File Format

Create markdown files named `vocabulary_XXX-YYY.md` with the following format:

```markdown
1. ephemeral /ɪˈfem(ə)rəl/
   - Lasting for a very short time
   - Transitory; soon passing away

2. serendipity /ˌserənˈdɪpəti/
   - The occurrence of events by chance in a happy way
   - Good fortune; luck
```

### Flashcard View

1. Open via ribbon icon (book icon) or command palette: "Open Vocabulary Flashcards"
2. Press **Space** to flip the card
3. Use **← →** arrow keys to navigate
4. Press **S** to shuffle

### Adding New Words

1. Click "Add Word" button or run command "Add New Word"
2. Enter the word
3. Click **Fetch from AI** to auto-fill pronunciation and definitions
4. Edit if needed and click **Add Word**

### LLM Configuration

Configure your AI provider in Settings → Vocabulary Flashcards:

| Provider | Default Endpoint | Default Model |
|----------|-----------------|---------------|
| DeepSeek | `https://api.deepseek.com/chat/completions` | `deepseek-chat` |
| OpenAI | `https://api.openai.com/v1/chat/completions` | `gpt-3.5-turbo` |
| Anthropic | `https://api.anthropic.com/v1/messages` | `claude-3-haiku` |
| Custom | User-defined | User-defined |

Enter your API key and customize the system prompt if needed.

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Space` | Flip card |
| `←` | Previous word |
| `→` | Next word |
| `S` | Shuffle cards |
| `/` | Open search |

## Commands

- `Open Vocabulary Flashcards` - Open the flashcard view
- `Search Vocabulary` - Open search modal
- `Add New Word` - Open add word modal
- `Reload Vocabulary Files` - Reload all vocabulary files

## License

MIT

## Contributing

Pull requests are welcome. For major changes, please open an issue first.
