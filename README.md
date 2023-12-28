# CODSOFT
To do list app
import java.util.ArrayList;
import java.util.List;

public class ToDoListApp {
    private List<Task> tasks;

    public ToDoListApp() {
        this.tasks = new ArrayList<>();
    }

    public void addTask(Task task) {
        tasks.add(task);
    }

    public void editTask(int index, Task updatedTask) {
        tasks.set(index, updatedTask);
    }

    public void markTaskAsCompleted(int index) {
        Task task = tasks.get(index);
        task.setCompleted(true);
    }

    public void deleteTask(int index) {
        tasks.remove(index);
    }

