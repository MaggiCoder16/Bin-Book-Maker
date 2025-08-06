
# PGN to BIN Book Converter

THIS FETCH_AND_BUILD.PY MAKES A PGN FILE FOR GOOD BOTS' CHESS960 GAMES. JUST RUN A WORKFLOW, YOU WILL GET ARTIFACT LINK TO DOWNLOAD .BIN BOOK.

This script takes a `.pgn` file containing chess games and converts it into a `.bin` Polyglot opening book, which can be used by engines and bots.

Fork this repository, upload a `.pgn` file, and name it exactly:

PgnFile.PGN

The script will read this file, process the games, and generate a `book.bin` as output. It supports both standard chess and Chess960, and filters games based on rating if needed.

The PGN must include `[FEN]` and `[SetUp "1"]` tags for Chess960 positions to be correctly handled.

The bookbuilder binary is expected to accept standard arguments for PGN input and BIN output.

The generated `book.bin` can be used directly in engines that support Polyglot books.

Feel free to contribute or suggest improvements.
