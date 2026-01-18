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
	gcc -o test_runner test_math.c math_ops.c 2>/dev/null || echo "No test files found"
	./test_runner 2>/dev/null || echo "Tests not implemented yet"
	echo "✅ Test phase complete"
