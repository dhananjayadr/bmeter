## Description
The bmeter plugin manager is a bash script designed to simplify the management of plugins for Apache JMeter. It provides functionalities to install, remove, list, and get information about plugins, as well as sync with a remote repository and restart JMeter.

### Why this exists? While there are existing solutions available for managing plugins in Apache JMeter.
Why not? It is fun.

## Prerequisites
- Apache JMeter installed
- `jq` JSON processor installed (can be installed via package manager like `pacman`, `brew`, or manually)
- `wget` installed for downloading files (usually pre-installed on most Unix like systems)

## Installation
1. Download the `bmeter` script.
2. Make the script executable:
   ```bash
   chmod +x bmeter
   ```

## Usage
```bash
./bmeter {-s|--install} [plugin_name] [plugin_version] | \
         {-r|--remove} [plugin_name] | \
         {-l|--list} | \
         {-i|--info} [plugin_name] | \
         {-y|--sync} | \
         {-R|--restart}
```

- `-s|--install [plugin_name] [plugin_version]`: Install a specific plugin with an optional version.
- `-r|--remove [plugin_name]`: Remove a plugin.
- `-l|--list`: List available plugins.
- `-i|--info [plugin_name]`: Get information about a specific plugin.
- `-y|--sync`: Sync with the remote repository to update the local plugin database.
- `-R|--restart`: Restart JMeter.
- `[plugin_name]`: Name of the plugin.
- `[plugin_version]`: Optional version of the plugin.

## To Do
1. Implement functionality to manage plugin dependencies.
2. Add support for removing installed plugins.
3. Explore options for packaging and distribution of this tool, possibly creating a package.
4. Enhance the script to support different platforms and package managers.
5. Allow users to specify and manage plugin versions during installation and removal.
6. Implement a feature to fetch and display a list of installed plugins.
7. Enhance the output formatting for better readability and user experience.
8. *(Add your own to-dos here)*

## License
This project is licensed under the [MIT License](LICENSE).

## Contribution
Contributions are welcome! If you find any bugs or have suggestions, please open an issue or create a pull request.
