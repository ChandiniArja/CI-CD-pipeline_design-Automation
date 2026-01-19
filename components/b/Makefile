# Simple Makefile for Component B

BIN=firmware_b.bin

all:
	echo "Building Component B..."
	touch $(BIN)
	echo "✅ Build complete"

clean:
	echo "Cleaning build files..."
	rm -f $(BIN) test_runner 2>/dev/null || true

test:
	echo "Running unit tests for Component B..."
	if ls test_*.c >/dev/null 2>&1; then \
		gcc -o test_runner test_*.c && \
		./test_runner; \
	else \
		echo "No test sources found, skipping tests"; \
	fi
	echo "✅ Test phase complete"
