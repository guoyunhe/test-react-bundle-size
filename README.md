# Test React & Preact bundle size and performance

## Test environment

- CPU: AMD Ryzen 5600X, 6 cores, 12 threads
- RAM: 4x8GB DDR4 3200MHz
- OS: openSUSE Tumbleweed, x86_64, kernel version 6.12.8
- Browser: Chromium 131, 20x cpu slow-down, slow 4G network throttling, cache disabled
- Bundler: Vite 6.x
- Server: `vite build && vite preview`

## Test result

| lib & version  | minified size | gzipped size | LCP   | INP  |
| -------------- | ------------- | ------------ | ----- | ---- |
| react 16.14.0  | 133.16 kB     | 41.92 kB     | 1.83s | 48ms |
| react 17.0.2   | 134.15 kB     | 43.45 kB     | 1.82s | 48ms |
| react 18.3.1   | 143.87 kB     | 46.34 kB     | 1.88s | 48ms |
| react 19.0.0   | 186.49 kB     | 58.96 kB     | 1.94s | 40ms |
| preact 10.25.4 | 16.26 kB      | 6.84 kB      | 1.71s | 16ms |
