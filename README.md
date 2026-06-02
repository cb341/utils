# Utils

Collection of web-based utilities for everyday tasks.

## Tools

### Estimator (PERT)
Three-point task estimation with confidence ranges, grounded in Robert C. Martin's
point in *The Clean Coder* that an estimate is a probability range, not a commitment.

**Features:**
- Optimistic / nominal / pessimistic per category (impl, review, testing, polish, client comms)
- PERT expected value (μ = (O+4N+P)/6) and combined uncertainty (σ = √Σσᵢ²)
- ~68% and ~95% confidence bands with a live bell curve
- Rough (optimistic-only) vs detailed two-phase workflow
- Newness multiplier for greenfield work, Fibonacci buckets, review-as-%-of-impl
- Live LaTeX formula rendering (KaTeX)
- Client-side only (no data sent to servers)

**Usage:** Open `estimator.html` in your browser.

### Discord Message Splitter
Split long messages into Discord-compatible chunks (2000/4000 character limits).

**Features:**
- Automatic splitting with newline awareness
- Collapsible preview (first/last 100 chars)
- Copy-to-clipboard with auto-hide
- Restore functionality
- Client-side only (no data sent to servers)

**Usage:** Open `discord_message_splitter.html` in your browser.

### Regex Intersection Checker
Find the smallest word that matches two regular expressions using NFAs.

**Features:**
- NFA simulation with Thompson's construction
- Pair comparison mode for checking two regexes
- Bulk uniqueness checking for multiple patterns
- SVG-based NFA visualization
- Supports literals, concatenation, alternation, Kleene star, plus, optional, and grouping
- Client-side only (no data sent to servers)

**Usage:** Open `regex_intersection_checker.html` in your browser.

## Running

All tools are standalone HTML files. Open directly in any modern browser.
Shared look-and-feel lives in `style.css` (a small self-contained stylesheet,
no framework).
