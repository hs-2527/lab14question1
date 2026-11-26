data class Student(val name: String, val percentage: Double, val department: String)

fun main() {
    // 1. Read-only and Mutable List
    println("----- LIST -----")
    val readOnlyList = listOf(10, 20, 30, 40)
    println("Read-only List: $readOnlyList")
    println("Contains 20: ${readOnlyList.contains(20)}")
    println("Get element at index 1: ${readOnlyList.get(1)}")

    val mutableList = mutableListOf(10, 20, 30, 40)
    mutableList.add(50)
    mutableList.remove(20)
    println("Mutable List after operations: $mutableList")

    // 2. Read-only and Mutable Set
    println("\\n----- SET -----")
    val readOnlySet = setOf(1, 2, 3, 4)
    println("Read-only Set: $readOnlySet")
    println("Contains 3: ${readOnlySet.contains(3)}")

    val mutableSet = mutableSetOf(1, 2, 3)
    mutableSet.add(4)
    mutableSet.remove(2)
    println("Mutable Set after operations: $mutableSet")

    // 3. Read-only and Mutable Map
    println("\\n----- MAP -----")
    val readOnlyMap = mapOf("A" to 90, "B" to 80)
    println("Read-only Map: $readOnlyMap")
    println("Get value of A: ${readOnlyMap.get("A")}")
    println("Contains key B: ${readOnlyMap.containsKey("B")}")

    val mutableMap = mutableMapOf("A" to 90, "B" to 80)
    mutableMap["C"] = 70
    mutableMap.remove("B")
    println("Mutable Map after operations: $mutableMap")

    // 4. Functional Transformations
    println("\\n----- FUNCTIONAL TRANSFORMATIONS -----")
    val numbers = listOf(1, 2, 3, 4, 5)

    val mapped = numbers.map { it * 2 }
    println("After map (multiply by 2): $mapped")

    val filtered = numbers.filter { it % 2 == 0 }
    println("After filter (even numbers): $filtered")

    val reduced = numbers.reduce { sum, number -> sum + number }
    println("After reduce (sum): $reduced")

    // 5. Sorting Student Objects
    println("\\n----- SORTING STUDENTS -----")
    val students = listOf(
        Student("Aman", 85.5, "CSE"),
        Student("Rohan", 92.0, "IT"),
        Student("Priya", 78.5, "CSE"),
        Student("Neha", 88.0, "IT")
    )

    val sortedStudents = students.sortedByDescending { it.percentage }
    println("Students sorted by percentage:")
    sortedStudents.forEach {
        println("${it.name} - ${it.percentage}%")
    }

    // 6. Grouping using groupBy
    println("\\n----- GROUPING STUDENTS -----")
    val groupedStudents = students.groupBy { it.department }
    groupedStudents.forEach { (department, studentList) ->
        println("$department: ${studentList.map { it.name }}")
    }
}
data class Student(val name: String, val percentage: Double, val department: String)

fun main() {
    // 1. Read-only and Mutable List
    println("----- LIST -----")
    val readOnlyList = listOf(10, 20, 30, 40)
    println("Read-only List: $readOnlyList")
    println("Contains 20: ${readOnlyList.contains(20)}")
    println("Get element at index 1: ${readOnlyList.get(1)}")

    val mutableList = mutableListOf(10, 20, 30, 40)
    mutableList.add(50)
    mutableList.remove(20)
    println("Mutable List after operations: $mutableList")

    // 2. Read-only and Mutable Set
    println("\\n----- SET -----")
    val readOnlySet = setOf(1, 2, 3, 4)
    println("Read-only Set: $readOnlySet")
    println("Contains 3: ${readOnlySet.contains(3)}")

    val mutableSet = mutableSetOf(1, 2, 3)
    mutableSet.add(4)
    mutableSet.remove(2)
    println("Mutable Set after operations: $mutableSet")

    // 3. Read-only and Mutable Map
    println("\\n----- MAP -----")
    val readOnlyMap = mapOf("A" to 90, "B" to 80)
    println("Read-only Map: $readOnlyMap")
    println("Get value of A: ${readOnlyMap.get("A")}")
    println("Contains key B: ${readOnlyMap.containsKey("B")}")

    val mutableMap = mutableMapOf("A" to 90, "B" to 80)
    mutableMap["C"] = 70
    mutableMap.remove("B")
    println("Mutable Map after operations: $mutableMap")

    // 4. Functional Transformations
    println("\\n----- FUNCTIONAL TRANSFORMATIONS -----")
    val numbers = listOf(1, 2, 3, 4, 5)

    val mapped = numbers.map { it * 2 }
    println("After map (multiply by 2): $mapped")

    val filtered = numbers.filter { it % 2 == 0 }
    println("After filter (even numbers): $filtered")

    val reduced = numbers.reduce { sum, number -> sum + number }
    println("After reduce (sum): $reduced")

    // 5. Sorting Student Objects
    println("\\n----- SORTING STUDENTS -----")
    val students = listOf(
        Student("Aman", 85.5, "CSE"),
        Student("Rohan", 92.0, "IT"),
        Student("Priya", 78.5, "CSE"),
        Student("Neha", 88.0, "IT")
    )

    val sortedStudents = students.sortedByDescending { it.percentage }
    println("Students sorted by percentage:")
    sortedStudents.forEach {
        println("${it.name} - ${it.percentage}%")
    }

    // 6. Grouping using groupBy
    println("\\n----- GROUPING STUDENTS -----")
    val groupedStudents = students.groupBy { it.department }
    groupedStudents.forEach { (department, studentList) ->
        println("$department: ${studentList.map { it.name }}")
    }
}
data class Student(val name: String, val percentage: Double, val department: String)

fun main() {
    // 1. Read-only and Mutable List
    println("----- LIST -----")
    val readOnlyList = listOf(10, 20, 30, 40)
    println("Read-only List: $readOnlyList")
    println("Contains 20: ${readOnlyList.contains(20)}")
    println("Get element at index 1: ${readOnlyList.get(1)}")

    val mutableList = mutableListOf(10, 20, 30, 40)
    mutableList.add(50)
    mutableList.remove(20)
    println("Mutable List after operations: $mutableList")

    // 2. Read-only and Mutable Set
    println("\\n----- SET -----")
    val readOnlySet = setOf(1, 2, 3, 4)
    println("Read-only Set: $readOnlySet")
    println("Contains 3: ${readOnlySet.contains(3)}")

    val mutableSet = mutableSetOf(1, 2, 3)
    mutableSet.add(4)
    mutableSet.remove(2)
    println("Mutable Set after operations: $mutableSet")

    // 3. Read-only and Mutable Map
    println("\\n----- MAP -----")
    val readOnlyMap = mapOf("A" to 90, "B" to 80)
    println("Read-only Map: $readOnlyMap")
    println("Get value of A: ${readOnlyMap.get("A")}")
    println("Contains key B: ${readOnlyMap.containsKey("B")}")

    val mutableMap = mutableMapOf("A" to 90, "B" to 80)
    mutableMap["C"] = 70
    mutableMap.remove("B")
    println("Mutable Map after operations: $mutableMap")

    // 4. Functional Transformations
    println("\\n----- FUNCTIONAL TRANSFORMATIONS -----")
    val numbers = listOf(1, 2, 3, 4, 5)

    val mapped = numbers.map { it * 2 }
    println("After map (multiply by 2): $mapped")

    val filtered = numbers.filter { it % 2 == 0 }
    println("After filter (even numbers): $filtered")

    val reduced = numbers.reduce { sum, number -> sum + number }
    println("After reduce (sum): $reduced")

    // 5. Sorting Student Objects
    println("\\n----- SORTING STUDENTS -----")
    val students = listOf(
        Student("Aman", 85.5, "CSE"),
        Student("Rohan", 92.0, "IT"),
        Student("Priya", 78.5, "CSE"),
        Student("Neha", 88.0, "IT")
    )

    val sortedStudents = students.sortedByDescending { it.percentage }
    println("Students sorted by percentage:")
    sortedStudents.forEach {
        println("${it.name} - ${it.percentage}%")
    }

    // 6. Grouping using groupBy
    println("\\n----- GROUPING STUDENTS -----")
    val groupedStudents = students.groupBy { it.department }
    groupedStudents.forEach { (department, studentList) ->
        println("$department: ${studentList.map { it.name }}")
    }
}
# lab14question1
