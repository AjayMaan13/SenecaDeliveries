# 🚚 Seneca Deliveries

[![C++](https://img.shields.io/badge/C++-11%2B-blue.svg)](https://en.cppreference.com/)
[![Testing](https://img.shields.io/badge/Tests-100%2B-brightgreen.svg)]()
[![Coverage](https://img.shields.io/badge/Coverage-100%25-success.svg)]()
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)

C/C++ delivery logistics system implementing route optimization algorithms and capacity management with comprehensive testing infrastructure demonstrating advanced QA methodologies.

## 🎯 Features

- 🚛 **Multi-Route Support** - Blue, Yellow, Green delivery routes with smart truck assignment
- 📦 **Package Validation** - Weight, size, destination verification with load balancing
- 🗺️ **Route Optimization** - Graph algorithms for efficient package delivery
- 🧪 **Comprehensive Testing** - 100+ test cases with multiple testing methodologies
- 🔍 **Quality Assurance** - Advanced testing strategies with full coverage analysis
- ⚡ **Performance Optimization** - Capacity constraints (2500kg, 100m³) management

## 🛠️ Tech Stack

**Core:** C/C++ with object-oriented design and modular architecture  
**Testing:** Microsoft Visual Studio Unit Test Framework, CppUnitTest.h  
**Algorithms:** Custom pathfinding, shortest path calculations, multi-criteria optimization  
**Data Structures:** Structs, arrays, pointers, dynamic memory management

## 🧪 Comprehensive Testing Infrastructure (100+ Test Cases)

### Testing Methodologies Implemented

**✅ White-Box Testing**
- Internal logic verification, code coverage analysis, path coverage, decision coverage

**⚫ Black-Box Testing**  
- Input boundary testing, equivalence partitioning, invalid input handling, output verification

**🔧 Unit Testing**
- Individual function isolation, mock data injection, return value verification, exception handling

**🔗 Integration Testing**
- Cross-module functionality validation, interface testing, data flow verification

**✅ Acceptance Testing**
- Business requirement validation, user story verification, end-to-end workflow testing

**🔄 Regression Testing**
- Automated test suite execution, version comparison, performance regression detection

**⚙️ Functional Testing**
- Core feature validation, business logic testing, input/output verification

**📊 Non-Functional Testing**
- Performance testing, memory optimization, scalability testing, reliability analysis

### Advanced QA Practices

- **Root Cause Analysis** - Systematic defect investigation and resolution
- **Traceability Matrix** - Requirements mapping to test cases
- **Quality Metrics** - Coverage analysis and defect density tracking
- **Test Documentation** - Comprehensive test plans and execution reports

## 🚀 Quick Start

### Build & Testing
```bash
# Open Visual Studio solution
Deliveries.sln

# Build configuration (Release/Debug x64)
MSBuild /p:Configuration=Release

# Run comprehensive test suite (100+ tests)
Test Explorer → Run All Tests

# Execute main application
./main.exe
```

### Usage
```bash
# Package entry format: weight size destination
450 3 12H    # 450kg, 3m³, destination 12H
0 0 x        # Stop entry
```

## 📁 Structure

```
Seneca-Polytechnic-Deliveries/
├── main.c                 # Application entry point
├── myFunctions.c/.h       # Core business logic
├── mapping.c/.h           # Route optimization algorithms
├── myHeader.h             # Data structure definitions
└── UnitTest/
    ├── UnitTest.cpp       # 100+ comprehensive test cases
    ├── TestFramework.h    # Testing infrastructure
    └── TestData/          # Test scenarios and data
```
### Testing Implementation
```c++
// Sample Test Structure
TEST_METHOD(TestTruckAssignment_Capacity) {
    // Arrange - Setup test data
    struct Truck trucks[3];
    struct PackageInfo package = {2000, 5, {12, 7}};
    
    // Act - Execute function
    int result = assignTruck(&package, trucks, 3);
    
    // Assert - Verify expected outcome
    Assert::IsTrue(result >= 0);
    Assert::IsTrue(trucks[result].currentWeight + 2000 <= MAX_WEIGHT);
}
```

## 📊 Quality Metrics & Achievements

- **100+ test cases** across all testing methodologies
- **100% code coverage** with comprehensive validation
- **Zero critical defects** through systematic testing approaches
- **Performance optimization** maintaining all capacity constraints
- **Complete SDLC implementation** from requirements to deployment

## 👨‍💻 Author

**Ajaypartap Singh Maan**  
[GitHub](https://github.com/AjayMaan13) • [LinkedIn](https://linkedin.com/in/ajaypartap-singh-maan) • ajayapsmaanm13@gmail.com

**Manas Gandotra**
[Linkedin](https://www.linkedin.com/in/manas-gandotra-627a69244/) • manasgandotra@gmail.com

---

⭐ **Star if helpful!**
