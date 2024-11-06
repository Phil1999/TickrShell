# TickrShell

TickrShell is a stock tracking CLI application designed using a microservices architecture. The project is split into multiple services, 
which work together to provide stock tracking functionality. These services include a CLI interface, a data service for fetching stock information,
and common components shared between them.

![Screenshot 2024-11-06 113821](https://github.com/user-attachments/assets/22b4eb16-7bcd-4555-8fa7-c7cb8999af18)



## Project Structure

This solution is split into three main projects:

- **StockTracker.CLI**: The command-line interface (CLI) for interacting with the stock tracking system. Users can issue commands to query stock prices, subscribe to updates, and display data in tabular or graphical formats.
- **StockTracker.Common**: This contains shared components used across the application, such as message definitions and database service abstractions.
- **StockTracker.DataService**: The service responsible for interacting with external stock APIs and managing stock data retrieval and updates.

## How to Clone the Project

This project uses Git submodules to manage the individual components, so you'll need to initialize and update the submodules when you first clone the repository.

### Steps to Clone and Setup:

1. Clone the main repository with submodules:
```bash
git clone --recurse-submodules https://github.com/Phil1999/TickrShell.git
```

2. If you've already cloned the repository without submodules, you can initialize them using:
```bash
git submodule update --init --recursive
```

3. Build the Project: Since this project is organized as a Visual Studio solution, simply open `StockApp.sln` in Visual Studio and build the solution. All submodules and components will be included automatically.

## Features

- **CLI-based**: A simple command-line interface for tracking and subscribing to stock updates.
- **Modular Design**: Designed using a microservices approach where each component has a distinct responsibility.
- **Extensible**: Easy to add new features such as additional stock data services or enhanced query functionalities.

## Submodules

This repository uses Git submodules to manage the separate components (StockTracker.CLI, StockTracker.Common, StockTracker.DataService). Each project is stored in its own directory and can be worked on individually or as part of the full solution.
