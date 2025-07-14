
```rust
// =========================================
//         Syaiful Imanudin :: Biodata.rs
// =========================================
//
// Compiling passion, curiosity, and code...
//

#[derive(Debug)]
struct Engineer {
    name: &'static str,
    experience: u8,
    stack: TechStack,
    passions: Vec<&'static str>,
    motto: &'static str,
}

#[derive(Debug)]
struct TechStack {
    backend: Vec<&'static str>,
    frontend: Vec<&'static str>,
    databases: Vec<&'static str>,
    message_brokers: Vec<&'static str>,
    tools: Vec<&'static str>,
}

fn main() {
    let syaiful = Engineer {
        name: "Syaiful Imanudin",
        experience: 3, // years
        stack: TechStack {
            backend: vec!["Go", "Java", "C#", "TypeScript", "Python", "PHP"],
            frontend: vec!["React", "TailwindCSS", "Bootstrap", "Next.js", "Astro"],
            databases: vec!["MySQL", "PostgreSQL", "Redis", "Microsoft SQL Server", "MongoDB"],
            message_brokers: vec!["RabbitMQ", "Kafka"],
            tools: vec!["Docker", "Kubernetes", "GCP", "AWS"],
        },
        passions: vec![
            "Designing robust APIs & microservices",
            "Building scalable backend architectures",
            "Crafting beautiful, responsive UIs",
            "Solving distributed systems challenges",
            "Automating cloud deployments & DevOps",
        ],
        motto: "Always ready for new challenges and building something extraordinary! 🚀",
    };

    println!("\nfn main() {{");
    println!("    // 👋 Hello, world!");
    println!("    let engineer = {{");
    println!("        name: {:?},", syaiful.name);
    println!("        experience: {}+ years,", syaiful.experience);
    println!("        tech_stack: {{");
    println!("            backend: {:?},", syaiful.stack.backend);
    println!("            frontend: {:?},", syaiful.stack.frontend);
    println!("            databases: {:?},", syaiful.stack.databases);
    println!("            message_brokers: {:?},", syaiful.stack.message_brokers);
    println!("            tools: {:?}", syaiful.stack.tools);
    println!("        }},");
    println!("        passions: [");
    for passion in syaiful.passions.iter() {
        println!("            - {}", passion);
    }
    println!("        ],");
    println!("        motto: {}", syaiful.motto);
    println!("    }}");
    println!("}}\n");
    println!("// Let's connect and build something awesome together! ✨");
}
```