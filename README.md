## rustlings 学习记录

> 注：此记录即为仓库的 commit message

commit 097237b9eabbd86c9d339d7aa6866942e07bfda4
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 16 11:01:34 2023 +0800

    update: tests9.rs
    
    - `extern` keyword declare the ABI when compile
    - `#[link_name = ".."]` change the linker's behavior
    - `#[no_mangle]` can be applied when we do not want rust compiler to change the name of a function
    
    authored by: Miao Hao

commit fe9c5509ed5d0ae1d915fcb5ef354ff127d9b12e
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 16 10:51:36 2023 +0800

    update: test[7-8].rs
    
    - build script are ran before project builds
    - can set pass some commands to cargo
    
    authored by: Miao Hao

commit 0e6e21c84210370ad903cdea867efac3f6524e31
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 16 10:26:55 2023 +0800

    update: test6.rs
    
    - create Box with raw pointer using `from_raw()` method
    
    authored by: Miao Hao

commit d3f1a174998f548b487dfc55f9497046f5c6c845
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 16 07:58:02 2023 +0800

    update: test5.rs
    
    - remove I AM NOT DONE
    
    authored by: Miao Hao

commit d4336c56654b8f44bc67c2c3a78c674b39a58501
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 16 07:56:19 2023 +0800

    update: test5.rs
    
    - raw pointers (*const T or *mut T) are derived from references, using `as` keyword
    - raw pointers are only allowed in `safe` blocks
    
    authored by: Miao Hao

commit f59233020ef8f3a8576c17cc5ac3da97727c8b23
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Sun Oct 15 17:18:56 2023 +0800

    update: convetsions/*.rs
    
    - from related traits can convert a type to another
    - AsRef and AsMut trait has methods to get a immutable/mutable reference
    
    authored by: Miao Hao

commit ac1a372b84f4d1d52df0fb3fbcc8e5bc30da2e50
Author: MiaoHao-oops <haomiao19@mails.ucas.ac.cn>
Date:   Sat Oct 14 23:00:42 2023 +0800

    update: using_as.rs, from_into.rs
    
    - use keyword `as` to convert a primitive type to another
    - impl `From` trait to convert a type to another
    
    authored by: Miao Hao

commit 82b456fae75770f03ec4361eef28d6e181273c12
Author: MiaoHao-oops <haomiao19@mails.ucas.ac.cn>
Date:   Sat Oct 14 22:30:41 2023 +0800

    update: clippy*.rs
    
    - clippy tool is a tool to give advice for incorrect rust code
    
    authored by: Miao Hao

commit b611e3015c7cea8e2683e512bea00a3e0bbc84ae
Author: MiaoHao-oops <haomiao19@mails.ucas.ac.cn>
Date:   Sat Oct 14 22:24:46 2023 +0800

    update: macros4.rs
    
    - remove I AM NOT DONE
    
    authored by: Miao Hao

commit 973341b01e6fc873c852ea4119fb2487f70f2fd4
Author: MiaoHao-oops <haomiao19@mails.ucas.ac.cn>
Date:   Sat Oct 14 22:23:32 2023 +0800

    update: macros*.rs
    
    - macro is the code to generate rust code
    - macro follows the rules of pattern matching
    
    authored by: Miao Hao

commit 81f1112e89495925fe6ea97e7b2294cff215ee21
Author: MiaoHao-oops <haomiao19@mails.ucas.ac.cn>
Date:   Sat Oct 14 22:10:14 2023 +0800

    update: threads*.rs
    
    - use `thread::spawn(f)` to creat a thread
    - use `handle.join()` to wait for a thread to finish and collect the
      return value
    - use `Arc`, `Mutex` to share data
    - use `std::sync::mpsc` to send message
    
    authored by: Miao Hao

commit d21ba28470ca0cc3f6c0b44524c95ec16607f9c2
Author: MiaoHao-oops <haomiao19@mails.ucas.ac.cn>
Date:   Sat Oct 14 20:59:55 2023 +0800

    update: cow1.rs
    
    - `Cow` stands for a copy-on-write smart pointer
    - when cow does not happend, `Cow` does not own the value, which for
      `Cow::Borrowed`
    - or it will own the value, for `Cow::Owned`
    
    authored by: Miao Hao

commit 1c96cde790f44385040b65d20e8a761e59d52f32
Author: MiaoHao-oops <haomiao19@mails.ucas.ac.cn>
Date:   Sat Oct 14 20:51:15 2023 +0800

    update: arc1.rs
    
    - use `Arc` to share data thread safely
    
    authored by: Miao Hao

commit 20204ae6ea9ea6e1de1e33425a41162ba21ad2b2
Author: MiaoHao-oops <haomiao19@mails.ucas.ac.cn>
Date:   Thu Oct 12 23:22:39 2023 +0800

    update: rc1.rs
    
    - `Rc<T>` stands for reference count, multiple variables have the
      ownership for one memory object
    - `Rc::clone()` will increase the count
    - variable leave scope will decrease the count
    
    authored by: Miao Hao

commit 990b5ae233cc16713d4b67c796373aa99a39b420
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Thu Oct 12 21:47:43 2023 +0800

    update: box1.rs
    
    - remove `I AM NOT DONE`
    
    authored by: Miao Hao

commit 7adf9d83247c3f64867e519b0a62d4507ba6860f
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Thu Oct 12 21:12:57 2023 +0800

    update: box1.rs
    
    - use `Box<T>` to solve recursive structure problems
    - use `Box::new()` to create objects on heap where `Box<T>` points to
    
    authored by: Miao Hao

commit a567c7270684b6cd32ac439c52f39de8e07abf6d
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Thu Oct 12 21:01:01 2023 +0800

    update: iterators[4-5].rs
    
    - `fold()` method reduce all items into a accumulator
    - `map()` method execute a closure on each item and generate a new iterator
    - `collect()` method collect items of an iterator and return a collection
    
    authored by: Miao Hao

commit ad318ad3837d0a702d297f460a4894dd112ef5cd
Author: MiaoHao-oops <haomiao19@mails.ucas.ac.cn>
Date:   Wed Oct 11 14:46:08 2023 +0800

    update: iterators3.rs
    
    - use collection methods
    
    authored by: Miao Hao

commit e55ea3db1c5d905316453565396cd51a085a77e0
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Tue Oct 10 22:38:41 2023 +0800

    update: iterators[1-2].rs
    
    - `iter()` on collection to create an iterator
    - `iter.next()` returns an Option
    
    authored by: Miao Hao

commit 88ba95e96a7e697e29a2cfb947b45117d4417fa0
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Tue Oct 10 11:17:18 2023 +0800

    update errors2.rs
    
    - add another solution: match statement
    
    authored by: Miao Hao

commit e3e22f9b6d0ebe287e721bfb67cd455315df46a6
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Tue Oct 10 09:59:06 2023 +0800

    update: tests[1-4].rs
    
    - write automate test in rust:
      - setup data
      - run functions you want to test
      - assert or check panic
    
    authored by: Miao Hao

commit 908850007fd9af0cee3708781409cb7c3f8dac5d
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Tue Oct 10 09:01:52 2023 +0800

    update: lifetimes3.rs
    
    - remove I AM NOT DONE
    
    authored by: Miao Hao

commit a6d0d7f0892e1e5fe6981dc7c40b1bf17431abbf
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Tue Oct 10 08:59:01 2023 +0800

    update: lifetime*.rs
    
    - each reference has a lifetime
    - lifetime for function or struct is a constraint
    - if the use of a function or a struct dose not meet the constraint, the compilse will report an error
    - a lifetime specifier takes the shortest lifetime for all references
    
    authored by: Miao Hao

commit db0cbcdf66ad8eb791072041f728ec26f1597217
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Tue Oct 10 08:26:46 2023 +0800

    update: quiz3.rs
    
    - there are two ways to bound a trait to a generic:
      - use `:` syntax after the generic `T`
      - use `where` clauses
    
    authored by: Miao Hao

commit 8a4f2768a7006b93f45f8eff8f107b03b7f368c0
Author: MiaoHao-oops <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 22:49:31 2023 +0800

    update: traits[4-5].rs
    
    - use `impl Trait` syntax to use traits as parameters
    - use `+` syntax to use more than one traits
    
    authored by: Miao Hao

commit 8db518ab30b80c2cdc0c8d6f8d71014e826fad13
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 22:40:25 2023 +0800

    update: traits[1-3].rs
    
    - trait is a shared behavior for different types
    - `Self` denotes for the certain type impl the trait
    - a function in a trait can be implemented in trait block or in impl block for a certain type
    
    authored by: Miao Hao

commit e52cf485a014c520632ab53e7b5f9a78a493c06c
Author: MiaoHao-oops <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 14:29:52 2023 +0800

    update: generics*.rs
    
    - `<T>`: declare a generics type
    - `impl<T>`: implement methods on generic
    
    authored by: Miao Hao

commit 7f2cfa80f3a3f7149ea990169ceba7b337a41ab5
Author: MiaoHao-oops <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 14:22:14 2023 +0800

    update: errors6.rs
    
    - `map_error()` method on Result can map a kind of error to another
    
    authored by: Miao Hao

commit ded7e3f44f92034c12a2959b92a5b3e6ef35cd91
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 13:54:19 2023 +0800

    update: errors[1-5].rs
    
    - `Result<T, E>` contains two variants: `Ok(T)` and `Err(E)` for error
    - `?` means return `Err(E)` for error and continue for `Ok(T)`
    
    authored by: Miao Hao

commit 168bd65415e36eade05882a56b190b46531af01d
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 11:12:56 2023 +0800

    update: options*.rs
    
    - use Option<T>::None to present `void`
    - `if let` and `while let` cares about only one case in `match`
    - `ref` keyword: bind by reference during pattern matching
    
    authored by: Miao Hao

commit 24e956cbce82671816f8f86e181b8ef96ca578c7
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 10:50:48 2023 +0800

    update: quiz2.rs
    
    authored by: Miao Hao

commit 839099a3aa7bb433821a98057d8f1b4ccd723794
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 10:10:12 2023 +0800

    update: hashmap*.rs
    
    - search for rust doc to use hashmaps
    
    authored by: Miao Hao

commit 934ed33837ff1ddc4a10f06c0764270488091962
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 10:01:59 2023 +0800

    update: modules*.rs
    
    - `use` keyword to bring a module path into scope
    - `pub` keyword to make an item in module public, private by default
    
    authored by: Miao Hao

commit 7c7676445918c1706728cd9b7d55673c74baf4b9
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 09:59:16 2023 +0800

    update: strings*.rs
    
    - `to_string` method on &str ccan change it to string
    - &str is the slice or reference of a string
    - conduct different methods on string
    
    authored by: Miao Hao

commit d06d2077ad08276394a664fdf691c71de3755fa6
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 09:54:00 2023 +0800

    update: info.toml
    
    - run `cargo install --path .` under root dir
    
    authored by: Miao Hao

commit 354771dda8889da90cb54d090d82f0c0bf9416db
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 09:45:51 2023 +0800

    update: enums*.rs
    
    - an enum contains several variants
    - variants in an enum can carry different values
    - a `match` statement can match variants for an enum, and grab the value
    
    authored by: Miao Hao

commit b3c9f819c89fd00b0348ace4d0a4d964ac240bf3
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 09:38:50 2023 +0800

    update: structs*.rs
    
    - 3 types of structs: classic, tuple, unit
    - define methods for a struct in `impl` block
    
    authored by: Miao Hao

commit b73fa517516b9ae2a054f3604d201f093e083e20
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 09:32:33 2023 +0800

    update: move_semantics*.rs
    
    - refer to rust documents
    
    authored by: Miao Hao

commit b8b9713b035b28ae2d261d53cdfc175c642afc37
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 09:26:57 2023 +0800

    update: vec*.rs
    
    - macro `vec![]` to create a vector and init
    - use `for` statement or collection method to traverse
    
    authored by: Miao Hao

commit 97338daf01a910eaa21ea419eba133bd2c37ab49
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 09:22:29 2023 +0800

    update: primitive_types*.rs
    
    - bool, char, array, tuple
    - `&name[1..b]` to grab a slice of an array
    - (x, y, ...) to destructure a tuple
    - name.x to extract a member of a tuple
    
    authored by: Miao Hao

commit 86ced2406311a20c9ed7236269dec6b05004485b
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 09:11:31 2023 +0800

    update: quiz1.rs
    
    authored by: Miao Hao

commit c39c6bf978b5143a733706f441a4fe1f974a4321
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 09:04:32 2023 +0800

    update: if*.rs
    
    - a C-like `if` statement
    - but can return a value
    - return values in a if stat should have same type
    
    authored by: Miao Hao

commit 6c4d3e2bdcb80c1c3fd9baeafe572a1c2791cac9
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 08:58:07 2023 +0800

    update: functions*.rs
    
    - declare a function: param type, return type `fn name(param1, ...) -> return type`
    - a line without `;` means return
    
    authored by: Miao Hao

commit 8c9816cb024851d4d0fce4ea30b07c37ff40c79b
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 08:55:24 2023 +0800

    update: variables*.rs
    
    - `let` keyword to bind a value to a variable
    - `:` to declare a type
    - `mut` keyword to make a variable mutable
    - a constant must be declared with a type
    
    authored by: Miao Hao

commit 73caaf6bdca2ab30b11d504bfaab341980d84dd6
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 08:52:31 2023 +0800

    update: intro2.rs
    
    - output `hello world` with rust
    
    authored by: Miao Hao

commit 5f076b84f04adb7cc7abccd37037e2b456120f6f
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 08:44:02 2023 +0800

    update: .gitignore
    
    - ignore origin rustlings repo
    
    authored by: Miao Hao

commit 93b4931cfe26d470242d402b7b0db4a8596dba84
Author: Miao Hao <haomiao19@mails.ucas.ac.cn>
Date:   Mon Oct 9 08:41:25 2023 +0800

    update: info.toml install.sh
    
    - clone from github stuck, create a mirror on gitee
    - rustlings run with panic, it cannot handle `buildscript`, replace it with `test`
    
    authored by: Miao Hao

commit be7d1916ec30ab86b4d24fecae22c74928fc8bbd
Author: github-classroom[bot] <66690702+github-classroom[bot]@users.noreply.github.com>
Date:   Sun Oct 8 23:52:56 2023 +0000

    add online IDE url

commit 4d0e9a71df22b4fcd355814a5920d9f1b4145bc0
Author: github-classroom[bot] <66690702+github-classroom[bot]@users.noreply.github.com>
Date:   Sun Oct 8 23:52:54 2023 +0000

    Initial commit
