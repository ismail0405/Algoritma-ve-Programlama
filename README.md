# Algoritma-ve-Programlama
Kod İşlem Süreleri

#include <iostream>
#include <ctime>
int main() {
clock_t start = clock();
std::cout << "Merhaba MIS, algoritma ve programlama \n";
clock_t end = clock();
double time_spent = (double)(end - start) /
CLOCKS_PER_SEC;
std::cout << "C++ işlem süresi: " << time_spent << "saniye\n";
return 0;
}

Merhaba MIS, algoritma ve programlama 
C++ işlem süresi: 4e-05saniye

#include <stdio.h>
#include <time.h>
int main() {
clock_t start = clock();
printf("Merhaba MIS, algoritma ve programlama\n");
clock_t end = clock();
double time_spent = (double)(end - start) /
CLOCKS_PER_SEC;
printf("C işlem süresi: %f saniye\n", time_spent);return 0;
}

Merhaba MIS, algoritma ve programlama
C işlem süresi: 0.000028 saniye


using System;
using System.Diagnostics;
class Program
{
static void Main()
{
Stopwatch stopwatch = new Stopwatch();
stopwatch.Start();
Console.WriteLine("Merhaba MIS, algoritma ve programlama dersi başladı");
stopwatch.Stop();
Console.WriteLine($"C# işlem süresi: {stopwatch.Elapsed.TotalSeconds} saniye");
}
}

Merhaba MIS, algoritma ve programlama dersi başladı
C# işlem süresi: 0.042641 saniye


public class Main {
public static void main(String[] args) {
long startTime = System.nanoTime();
System.out.println("Merhaba MIS, algoritma ve programlama dersi başladı");
long endTime = System.nanoTime();
double duration = (endTime - startTime) /
1_000_000.0; // milisaniye cinsine çevir
System.out.println("Java işlem süresi: " + duration + "milisaniye");
}
}

Merhaba MIS, algoritma ve programlama dersi başladı
Java işlem süresi: 0.428752milisaniye

const startTime = process.hrtime();
console.log("Merhaba MIS, algoritma ve programlama dersi başladı");
const endTime = process.hrtime(startTime);
const duration = endTime[0] * 1e3 + endTime[1] / 1e6; //milisaniye cinsine çevir
console.log(`JavaScript işlem süresi: ${duration.toFixed(3)}milisaniye`);

Merhaba MIS, algoritma ve programlama dersibaşladı
JavaScript işlem süresi: 4.719milisaniye

package main
import (
"fmt"
"time"
)
func main() {
start := time.Now()
fmt.Println("Merhaba MIS, algoritma ve programlama")
elapsed := time.Since(start)
fmt.Printf("Go işlem süresi: %s saniye\n", elapsed)
}

Merhaba MIS, algoritma ve programlama
Go işlem süresi: 26.223µs saniye


use std::time::Instant;
fn main() {
let start = Instant::now();
println!("Merhaba MIS, algoritma ve programlama");
let duration = start.elapsed();
println!("Rust işlem süresi: {:?}", duration);
}

Merhaba MIS, algoritma ve programlama
Rust işlem süresi: 12.874µs

start = Time.now
puts "Merhaba MIS, algoritma ve programlama"
finish = Time.now
puts "Ruby işlem süresi: #{finish - start} saniye"

Merhaba MIS, algoritma ve programlama
Ruby işlem süresi: 2.019e-05 saniye

use Time::HiRes qw(time);
my $start = time();
print "Merhaba MIS, algoritma ve programlama\n";
my $end = time();
printf "Perl işlem süresi: %f saniye\n", $end - $start;

Merhaba MIS, algoritma ve programlama
Perl işlem süresi: 0.000013 saniye

import time
start = time.time()
print("Merhaba MIS, algoritma ve programlama dersi başladı")
end = time.time()
print(f"Python işlem süresi: {end - start} saniye")

Merhaba MIS, algoritma ve programlama dersi başladı
Python işlem süresi: 2.0742416381835938e-05 saniye
