#
```
[0x00400860]> pdf @ main
            ; DATA XREF from entry0 @ 0x40087d
┌ 208: int main (int argc, char **argv, char **envp);
│           ; var int64_t var_14h @ rbp-0x14
│           ; var int64_t var_10h @ rbp-0x10
│           ; var int64_t var_ch @ rbp-0xc
│           ; var void *ptr @ rbp-0x8
│           0x00400b1e      55             push rbp
│           0x00400b1f      4889e5         mov rbp, rsp
│           0x00400b22      4883ec20       sub rsp, 0x20
│           0x00400b26      c745f4000000.  mov dword [var_ch], 0
│           0x00400b2d      c745f0000000.  mov dword [var_10h], 0
│           0x00400b34      c745ec000000.  mov dword [var_14h], 0
│           0x00400b3b      bed00c4000     mov esi, str.Enter_three_numbers ; 0x400cd0 ; "Enter three numbers!\n"
│           0x00400b40      bfa0216000     mov edi, obj.std::cout      ; 0x6021a0
│           0x00400b45      e8e6fcffff     call sym std::basic_ostream<char, std::char_traits<char> >& std::operator<< <std::char_traits<char> >(std::basic_ostream<char, std::char_traits<char> >&, char const*) ; sym.imp.std::basic_ostream_char__std::char_traits_char_____std::operator____std::char_traits_char____std::basic_ostream_char__std::char_traits_char______char_const
│           0x00400b4a      488d45f4       lea rax, [var_ch]
│           0x00400b4e      4889c6         mov rsi, rax
│           0x00400b51      bf80206000     mov edi, obj.std::cin       ; sym..bss
│                                                                      ; 0x602080
│           0x00400b56      e8f5fcffff     call sym std::istream::operator>>(int&) ; sym.imp.std::istream::operator___int
│           0x00400b5b      488d55f0       lea rdx, [var_10h]
│           0x00400b5f      4889d6         mov rsi, rdx
│           0x00400b62      4889c7         mov rdi, rax
│           0x00400b65      e8e6fcffff     call sym std::istream::operator>>(int&) ; sym.imp.std::istream::operator___int
│           0x00400b6a      488d55ec       lea rdx, [var_14h]
│           0x00400b6e      4889d6         mov rsi, rdx
│           0x00400b71      4889c7         mov rdi, rax
│           0x00400b74      e8d7fcffff     call sym std::istream::operator>>(int&) ; sym.imp.std::istream::operator___int
│           0x00400b79      8b55f4         mov edx, dword [var_ch]
│           0x00400b7c      8b45f0         mov eax, dword [var_10h]
│           0x00400b7f      01c2           add edx, eax
│           0x00400b81      8b45ec         mov eax, dword [var_14h]
│           0x00400b84      01d0           add eax, edx
│           0x00400b86      89c7           mov edi, eax
│           0x00400b88      e8c0fdffff     call sym gen(int)           ; sym.gen_int
│           0x00400b8d      488945f8       mov qword [ptr], rax
│           0x00400b91      8b55f4         mov edx, dword [var_ch]
│           0x00400b94      8b45f0         mov eax, dword [var_10h]
│           0x00400b97      01c2           add edx, eax
│           0x00400b99      8b45ec         mov eax, dword [var_14h]
│           0x00400b9c      01d0           add eax, edx
│           0x00400b9e      3d39050000     cmp eax, 0x539              ; 1337
│       ┌─< 0x00400ba3      7527           jne 0x400bcc
│       │   0x00400ba5      bee60c4000     mov esi, str.easyctf        ; 0x400ce6 ; "easyctf{"
│       │   0x00400baa      bfa0216000     mov edi, obj.std::cout      ; 0x6021a0
│       │   0x00400baf      e87cfcffff     call sym std::basic_ostream<char, std::char_traits<char> >& std::operator<< <std::char_traits<char> >(std::basic_ostream<char, std::char_traits<char> >&, char const*) ; sym.imp.std::basic_ostream_char__std::char_traits_char_____std::operator____std::char_traits_char____std::basic_ostream_char__std::char_traits_char______char_const
│       │   0x00400bb4      488b45f8       mov rax, qword [ptr]
│       │   0x00400bb8      4889c7         mov rdi, rax
│       │   0x00400bbb      e823ffffff     call sym print_ptr(char*)   ; sym.print_ptr_char
│       │   0x00400bc0      bfef0c4000     mov edi, 0x400cef           ; const char *s
│       │   0x00400bc5      e8f6fbffff     call sym.imp.puts           ; int puts(const char *s)
│      ┌──< 0x00400bca      eb0f           jmp 0x400bdb
│      ││   ; CODE XREF from main @ 0x400ba3
│      │└─> 0x00400bcc      bef10c4000     mov esi, str.nope.          ; 0x400cf1 ; "nope.\n"
│      │    0x00400bd1      bfa0216000     mov edi, obj.std::cout      ; 0x6021a0
│      │    0x00400bd6      e855fcffff     call sym std::basic_ostream<char, std::char_traits<char> >& std::operator<< <std::char_traits<char> >(std::basic_ostream<char, std::char_traits<char> >&, char const*) ; sym.imp.std::basic_ostream_char__std::char_traits_char_____std::operator____std::char_traits_char____std::basic_ostream_char__std::char_traits_char______char_const
│      │    ; CODE XREF from main @ 0x400bca
│      └──> 0x00400bdb      488b45f8       mov rax, qword [ptr]
│           0x00400bdf      4889c7         mov rdi, rax                ; void *ptr
│           0x00400be2      e859fcffff     call sym.imp.free           ; void free(void *ptr)
│           0x00400be7      b800000000     mov eax, 0
│           0x00400bec      c9             leave
└           0x00400bed      c3             ret
```
