poison null byte to create overlapping chunks with no heap leak i assume the address ends with \x00\x00 (requires 1 nibble brute force), then use the double free (overlapping chunks) to perform tcache dump 