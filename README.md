# Python_AI Projects

This is a parent repository that aggregates multiple Python AI projects as git submodules.

## Structure

This repository contains the following submodules:

- **savnet-python-ai** - Semi-theoretical course lessons with examples and tasks for all 4 modules of the ZF+Savnet Python and AI Academy
- **MyWork** - Homework assignments, mini-projects, and personal work completed for the ZF+Savnet Python and AI Academy
- **ZF_Savnet_City_Bike_Project** - Well-documented project for the academy

## Getting Started

### Cloning the Repository

To clone this repository along with all submodules:

```bash
git clone --recursive <repository-url>
```

If you've already cloned without the `--recursive` flag, initialize submodules:

```bash
git submodule init
git submodule update
```

Or combine both:

```bash
git submodule update --init --recursive
```

### Working with Submodules

#### Updating Submodules

To update all submodules to their latest commits:

```bash
git submodule update --remote
```

To update a specific submodule:

```bash
git submodule update --remote <submodule-name>
```

#### Making Changes to a Submodule

1. Navigate to the submodule directory:
   ```bash
   cd savnet-python-ai
   ```

2. Make your changes, commit, and push to the submodule's remote:
   ```bash
   git add .
   git commit -m "Your changes"
   git push
   ```

3. Go back to the parent repository and update the submodule reference:
   ```bash
   cd ..
   git add savnet-python-ai
   git commit -m "Update savnet-python-ai submodule"
   git push
   ```

#### Checking Submodule Status

To see the status of all submodules:

```bash
git submodule status
```

## Project Overview

This repository contains all code and work completed for the ZF+Savnet Python and AI Academy. It serves as a centralized hub for the various projects, assignments, and learning materials from the academy. Each submodule maintains its own version control history and can be developed independently while being tracked together at specific commit points.

## Additional Projects

In addition to the submodules listed above, there is a separate large-scale private project developed for ZF company that is not included in this repository due to its confidential nature and size. This project is maintained independently and is not tracked as part of this public repository.
