Welcome to the start of your TDD journey. Please be patient as your enviorment loads, it usually takes less than a minute.

## TDD Starts with a test file

TDD starts with testing before any development.

Open the file `src/test/java/StudentTest.java`{{open}}.

As you can see there's not not much here yet, our first task is to write our first test.

## Write your first test

Write your first test to define what you'd like to happen, this is what you expect to happen once the code has been written.

For our first test we're going to create a `StudentTest` class and create a test that asserts that StudentName is not null when we call our Student function (note there's no code in our studnet function so we expect this test will fail).

Copy the following into the editor by hitting 'copy to editor' RELATIVE_PATH:

<pre class="file" data-filename="src/test/java/StudentTest.java" data-target="replace">
import org.junit.jupiter.api.Test;
import static org.junit.jupiter.api.Assertions.*;
import com.Student;
public class StudentTest {
  @Test
  public void whenStudentNameSuppliedStringReturned() {
    name=Student.name('bob')
    assertNotEquals("", name);
  }
}
</pre>

## Run your first test (Red)

Let's now run our test! We're expecting that this will be "red" or "fail" as we've only written the test (we'll make it pass in the next step).

Click execute to run your first test:

`bash ./gradlew test`{{execute}}

Now you're ready for the part everyone loves, making things green! Click continue when you're ready.
