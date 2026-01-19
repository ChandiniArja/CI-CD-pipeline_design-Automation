# Simple Makefile for Component A
all:
	echo "Building Component A..."
	touch firmware_a.bin
	echo "✅ Build complete"

clean:
	echo "Cleaning build files..."
	rm -f firmware_a.bin 2>/dev/null || true

test:
	echo "Running unit tests for Component A..."
	if [ -f test_math.c ] && [ -f math_ops.c ]; then \
		gcc -o test_runner test_math.c math_ops.c && \
		./test_runner; \
	else \
		echo "No test sources found, skipping tests"; \
	fi
	echo "✅ Test phase complete"
